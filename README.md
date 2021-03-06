# Smicro PHP Micro-framework

Micro-framework based on Symfony - Fast micro-services and APIs delivered with the elegance you expect.

Smicro is the perfect solution for building Symfony based micro-services and fast APIs. In fact, it's nearly twice as fast as Symfony Standard.

[![Build Status](https://travis-ci.org/sgasser/smicro.svg?branch=master)](https://travis-ci.org/sgasser/smicro)
[![Packagist](https://img.shields.io/packagist/v/sgasser/smicro.svg)](https://packagist.org/packages/sgasser/smicro)
[![Installs](https://img.shields.io/packagist/dt/sgasser/smicro.svg)](https://packagist.org/packages/sgasser/smicro)
[![license](https://img.shields.io/github/license/sgasser/smicro.svg)](<https://github.com/sgasser/smicro/blob/master/LICENSE>)
[![SensioLabsInsight](https://insight.sensiolabs.com/projects/12e42ff3-5bd2-4241-9e7a-5fe8d6e330ec/mini.png)](https://insight.sensiolabs.com/projects/12e42ff3-5bd2-4241-9e7a-5fe8d6e330ec)

# What's included

Symfony3 with MicroKernel using [MicroKernelTrait](http://symfony.com/doc/current/configuration/micro_kernel_trait.html)

## Bundles registered in the MicroKernel

- FrameworkBundle
- MonologBundle
- WebProfilerBundle (DEV)

## Create project

```
composer create-project sgasser/smicro
```

# Usage

## Structure - common files

- app
  - config
    - routing.yml
    - services.yml
- src
- tests

## Start local server

```
php bin/console server:run
```

## Run tests

```
vendor/bin/phpunit
```

# Deploy

Smicro is ready for the cloud

## Heroku

Visit <http://heroku.com/> to set up an account.

Initialize local GIT

```
git init
git add .
git commit -m 'Initial commit'
```

Create heroku app

```
heroku create
```

Set config

```
heroku config:set SYMFONY_ENV=prod
```

Push

```
git push heroku master
```

Open app

```
heroku open
```
