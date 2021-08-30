Rails Bootstrap Examples (Album)
================================

[![Build status][shield-build]](#)
[![MIT licensed][shield-license]](#)
[![Rails][shield-rails]][rails]

Rails 6 に Bootstrap 4 の Examples (Album) を組み込んだサンプル。

https://getbootstrap.com/docs/4.6/examples/album/

## Table of Contents

* [Technologies](#technologies)
* [Demo](#demo)
* [Getting started](#getting-started)
* [Deployment](#deployment)
* [Usage](#usage)
* [References](#references)
* [License](#license)

## Technologies

* [Rails][rails] 6.0.4.1
* [Bootstrap](https://getbootstrap.com/) 4.6
* [PostgreSQL][postgresql]
* [Heroku][heroku]

## Demo

* [Heroku](https://kyuuki-sample-rails-album.herokuapp.com)

## Getting started

### Rails アプリケーション作成

```sh
$ git clone git@github.com:kyuuki/sample-rails-bootstrap.git sample-rails-bootstrap-examples-album
$ cd sample-rails-bootstrap-examples-album/
```

### Examples (Album) 組み込み

- [[commit]](https://github.com/kyuuki/sample-rails-bootstrap-examples-album/commit/a0ac04d90b0211fe85bc0db65a95009d4de11749)

### GitHub

- GitHub に sample-rails-bootstrap-examples-album という名前でリポジトリ追加

```sh
$ git remote set-url origin git@github.com:kyuuki/sample-rails-bootstrap-examples-album.git
$ git push origin master
```

## Deployment

Heroku にデプロイ

```sh
$ heroku create kyuuki-sample-rails-album (maximum is 30 characters)
$ git push heroku master
```
<!-- $ heroku run rake db:migrate (今回は不要) -->

## Usage

```sh
$ git clone git@github.com:kyuuki/sample-rails-bootstrap-examples-album.git
$ cd sample-rails-bootstrap-examples-album
$ bundle install
$ yarn install
$ rails db:create
$ rails s -b 0.0.0.0
```
<!-- $ rails db:migrate (今回は不要) -->

## References

* [Bootstrap 4.6 Documentation](https://getbootstrap.com/docs/4.6/)

## License

This is licensed under the [MIT](https://choosealicense.com/licenses/mit/) license.  
Copyright &copy; 2021 [Fuji Programming Laboratory](https://fuji-labo.com/)



[rails]: https://rubyonrails.org/
[postgresql]: https://www.postgresql.org/
[heroku]: https://www.heroku.com/home

[shield-build]: https://img.shields.io/badge/build-passing-brightgreen.svg
[shield-license]: https://img.shields.io/badge/license-MIT-blue.svg
[shield-rails]: https://img.shields.io/badge/-Rails-CC0000.svg?logo=ruby-on-rails&style=flat
