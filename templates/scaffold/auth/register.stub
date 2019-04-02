@extends('layouts.app')

@section('content')
    <div class="container">
        <div class="row">
            <div class="col-sm-9 col-md-7 col-lg-5 mx-auto">
                <div class="card my-5">
                    <div class="card-body">
                        <h5 class="card-title text-center">Register</h5>
                        <form role="form" method="POST" action="{{ url('/register') }}">
                            {!! csrf_field() !!}
                            <div class="form-label-group {{ $errors->has('name') ? ' has-error' : '' }}">
                                <label for="inputName">Name</label>
                                <input type="text" id="inputName" class="form-control" placeholder="Name"
                                       required autofocus name="name" value="{{ old('name') }}">
                                @if ($errors->has('name'))
                                    <span class="help-block">
                                  <strong>{{ $errors->first('name') }}</strong>
                                </span>
                                @endif
                            </div>

                            <div class="form-label-group mt-2 {{ $errors->has('email') ? ' has-error' : '' }}">
                                <label for="inputEmail">Email address</label>
                                <input type="email" id="inputEmail" class="form-control" placeholder="E-Mail Address"
                                       required name="email" value="{{ old('email') }}">
                                @if ($errors->has('email'))
                                    <span class="help-block">
                                  <strong>{{ $errors->first('email') }}</strong>
                                </span>
                                @endif
                            </div>

                            <div class="form-label-group mt-2 {{ $errors->has('password') ? ' has-error' : '' }}">
                                <label for="inputPassword">Password</label>
                                <input type="password" name="password" id="inputPassword" class="form-control"
                                       placeholder="Password"
                                       required>
                                @if ($errors->has('password'))
                                    <span class="help-block">
                                        <strong>{{ $errors->first('password') }}</strong>
                                    </span>
                                @endif
                            </div>

                            <div
                                class="form-label-group mb-3 mt-2 {{ $errors->has('password_confirmation') ? ' has-error' : '' }}">
                                <label for="inputConfirmPassword">Confirm Password</label>
                                <input type="password" name="password_confirmation" id="inputConfirmPassword"
                                       class="form-control"
                                       placeholder="Password"
                                       required>
                                @if ($errors->has('password_confirmation'))
                                    <span class="help-block">
                                        <strong>{{ $errors->first('password_confirmation') }}</strong>
                                    </span>
                                @endif
                            </div>
                            <button class="btn btn-lg btn-primary btn-block text-uppercase" type="submit">Register
                            </button>
                            <a class="btn btn-link" href="{{ url('/login') }}">Already account?</a>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </div>
@endsection
