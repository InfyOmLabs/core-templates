@extends('layouts.app')

@section('content')
    <div class="container">
        <div class="row">
            <div class="col-sm-9 col-md-7 col-lg-5 mx-auto">
                <div class="card my-5">
                    <div class="card-body">
                        <h5 class="card-title text-center">Sign In</h5>
                        <form role="form" method="POST" action="{{ url('/login') }}">
                            {!! csrf_field() !!}
                            <div class="form-label-group">
                                <label for="inputEmail">Email address</label>
                                <input type="email" id="inputEmail" class="form-control" placeholder="Email address"
                                       required autofocus name="email" value="{{ old('email') }}">
                                @if ($errors->has('email'))
                                    <span class="help-block">
                                        <strong>{{ $errors->first('email') }}</strong>
                                    </span>
                                @endif
                            </div>

                            <div class="form-label-group mt-2">
                                <label for="inputPassword">Password</label>
                                <input type="password" name="password" id="inputPassword" class="form-control"
                                       placeholder="Password"
                                       required>
                            </div>

                            <div class="custom-control custom-checkbox mb-3 mt-3">
                                <input type="checkbox" class="custom-control-input" name="remember" id="customCheck1">
                                <label class="custom-control-label" for="customCheck1">Remember Me</label>
                            </div>
                            <button class="btn btn-lg btn-primary btn-block text-uppercase" type="submit">Login</button>
                            <a class="btn btn-link" href="{{ url('/password/reset') }}">Forgot Your Password?</a>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </div>
@endsection
