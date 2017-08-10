# go-laravel-echo

A Golang server for Laravel Echo using Server-Sent Events.

Inspired by [tlaverdure/laravel-echo-server](https://github.com/tlaverdure/laravel-echo-server) (NodeJS).

## System Requirements

The following are required to function properly.

*   Laravel 5.3+
*   Redis 3+

Additional information on broadcasting with Laravel can be found on the
official docs: <https://laravel.com/docs/master/broadcasting>

## Getting Started

TODO

## Configuration

Configuration is done using Environment variables or the Laravel `.env` file.

Here are the defaults:

| Title            | Default              | Description                 |
| :--------------- | :------------------- | :---------------------------|
| `authEndpoint`   | `/broadcasting/auth` | The route that authenticates private channels  |
| `authHost`       | `http://localhost`   | The host of the server that authenticates private and presence channels  |
| `database`       | `redis`              | Database used to store data that should persist, like presence channel members. Currently only `redis` is supported |
| `databaseConfig` |  `{}`                | Configurations for the different database drivers [Example](#database)|
| `host`           | `null`               | The host this service should listen on ex.`app.dev`. `null` will accept connections on any address |
| `port`           | `6001`               | The port that the server should run on |
| `protocol`       | `http`               | either `http` or `https` |
| `sslCertPath`    | `''`                 | The path to your server's ssl certificate |
| `sslKeyPath`     | `''`                 | The path to your server's ssl key |
| `sslPassphrase`  | `''`                 | The pass phrase to use for the certificate (if applicable) |
