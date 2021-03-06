# Browserlog

[![Build Status](https://travis-ci.org/dieb/browserlog.svg?branch=master)](https://travis-ci.org/dieb/browserlog)
[![Dependency Status](https://img.shields.io/gemnasium/dieb/browserlog.svg)][gemnasium]
[![Code Climate](https://img.shields.io/codeclimate/github/dieb/browserlog.svg)][codeclimate]
[![Coverage Status](https://coveralls.io/repos/dieb/browserlog/badge.png?branch=master)](https://coveralls.io/r/dieb/browserlog?branch=master)

[travis]: http://travis-ci.org/dieb/browserlog
[gemnasium]: https://gemnasium.com/dieb/browserlog
[codeclimate]: https://codeclimate.com/github/dieb/browserlog
[coveralls]: https://coveralls.io/r/dieb/browserlog

Browserlog is a live web log viewer for rails apps.

![Screenshot dark theme](https://dl.dropboxusercontent.com/u/27144161/browserlog-dark.png "Screenshot dark theme")
![Screenshot light theme](https://dl.dropboxusercontent.com/u/27144161/browserlog-light.png "Screenshot light theme")

## Features
* Auto-refresh

## Installation

The simplest way to install Browserlog is to use [Bundler](http://bundler.io).

```ruby
gem 'browserlog', '~> 0.0.1', git: 'https://github.com/dieb/browserlog.git'
```

Browserlog is bundled as a Rails engine. Mount it on `config/routes.rb`.

```ruby
MyApp::Application.routes.draw do
  mount Browserlog::Engine => '/logs'
end
```

With this setup 'logs/development', 'logs/production' and 'logs/test' are automatically available.

## Supported Rails Versions
* Rails ~> 4.1.0
