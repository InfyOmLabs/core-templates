@extends('layouts.app')

<!-- Main Content -->
@section('content')
    <div class="container">
        <div class="row">
            <div class="col-sm-9 col-md-7 col-lg-5 mx-auto">
                <div class="card my-5">
                    <div class="card-body">
                        @if (session('status'))
                            <div class="alert alert-success">
                                {{ session('status') }}
                            </div>
                        @endif
                        <h5 class="card-title text-center">Reset Password</h5>
                        <form role="form" method="POST" action="{{ url('/password/email') }}">
                            {!! csrf_field() !!}
                            <input type="hidden" name="token" value="{{ $token }}">

                            <div class="form-label-group my-2 {{ $errors->has('email') ? ' has-error' : '' }}">
                                <label for="inputEmail">Email address</label>
                                <input type="email" id="inputEmail" class="form-control" placeholder="E-Mail Address"
                                       required name="email" value="{{ old('email') }}">
                                @if ($errors->has('email'))
                                    <span class="help-block">
                                  <strong>{{ $errors->first('email') }}</strong>
                                </span>
                                @endif
                            </div>
                            <button class="btn btn-lg btn-primary btn-block" type="submit">
                                <i class="fa fa-btn fa-envelope"></i> Send Password Reset Link
                            </button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </div>
@endsection
