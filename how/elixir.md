# Erlang and Elixir

The `erlang` and `elixir` packages found in the standard repository typically quite old.

Rabbit MQ offers a fork of the official Erlang and Elixir packages for Debian. 

This repository targets the oldest version supported by currently developed release series.

```
add-apt-repository -P rabbitmq/rabbitmq-erlang
```
Add the rabbitmq source.
```
apt update
```
Fetch source.
```
apt install erlang elixir
```
Install latest version of `erlang` and `elixir`.

```
elixir -v

Erlang/OTP 27 [erts-15.2.7.4]  ...

Elixir 1.17.3 (compiled with Erlang/OTP 26)
```
Done!