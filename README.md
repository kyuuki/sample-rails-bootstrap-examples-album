Rails Bootstrap サンプル
========================

[![Build status][shield-build]](#)
[![MIT licensed][shield-license]](#)
[![Rails][shield-rails]][rails]

Rails 6 に Bootstrap 4 を導入するサンプル。

CDN を利用してお手軽に導入する方法。

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

* [Heroku](https://kyuuki-sample-rails-bootstrap.herokuapp.com)

## Getting started

### Rails アプリケーション作成

```sh
$ git clone git@github.com:kyuuki/sample-rails-base.git sample-rails-bootstrap
$ cd sample-rails-bootstrap
```

### Bootstrap 導入

- [Starter template](https://getbootstrap.com/docs/4.6/getting-started/introduction/#starter-template) を参考に [app/views/layouts/application.html.erb](app/views/layouts/application.html.erb) を編集  
  [[commit]](https://github.com/kyuuki/sample-rails-bootstrap/commit/cc0c6712c65a2ae34371dd804a846da8e03e2bcd)

### トップページにボタンを追加して確認

- [app/views/static_page/top.html.erb](app/views/static_page/top.html.erb) にボタンを追加して、Bootstrap が適用できたか確認

```erb
<h1>トップページ</h1>

<p>
  トップページの内容。
</p>

<button type="button" class="btn btn-primary">Primary</button> ← 追加
```

### GitHub

- GitHub に sample-rails-bootstrap という名前でリポジトリ追加

```sh
$ git remote set-url origin git@github.com:kyuuki/sample-rails-bootstrap.git
$ git push origin master
```

## Deployment

Heroku にデプロイ

```sh
$ heroku create kyuuki-sample-rails-bootstrap
$ git push heroku master
```
<!-- $ heroku run rake db:migrate (今回は不要) -->

## Usage

```sh
$ git clone git@github.com:kyuuki/sample-rails-bootstrap.git
$ cd sample-rails-bootstrap
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
