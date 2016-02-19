# Felt
Front end load testing with PhantomJS/SlimerJS, sponsored by [CoScale](http://www.coscale.com)

## Description
Felt is a front-end load tester. It generates load by running a lot of browser instances simultaneously and waiting for the page to finish loading (no more pending resource calls). The tool uses [PhantomJS](http://phantomjs.org/) or [SlimerJS](https://slimerjs.org/). You can use Felt to quickly generate load on front end heavy applications. With  scenarios you can setup a path through your application for the browsers to follow.

## Use cases

* Load testing
    * AngularJS
    * React
    * Backbone.js
    * Ember.js
* Cache warming
* Quick local load tests

## Features

* Real browser load testing of web applications
* Works with PhantomJS (webkit) and SlimerJS (firefox)
* Scenarios
* Performance statistics **(TODO)**
* Statistics **(TODO)**
* Multi machine load testing **(TODO)**

## Requirements

* Tested on Python 2.7.10
* Unix based operating system
* Local install of [PhantomJS](http://phantomjs.org/download.html) or [SlimerJS](https://slimerjs.org/download.html) available in PATH

## Quick start

1. `git clone https://github.com/kidk/felt.git`
1. `cd felt`
1. Download PhantomJS from http://phantomjs.org/download.html
1. Unzip and move PhantomJS executable into felt directory

    The felt directory should look something like this:
        $ ls
        LICENSE		README.md	js		main.py		phantomjs

1. `python main.py --verbose examples/basic.json`
1. `ctrl + c` to stop

## Usage
```
usage: main.py [-h] [--debug] [--verbose] [--threads THREADS] [--test]
               scenario

Start workload.

positional arguments:
  scenario

optional arguments:
  -h, --help         show this help message and exit
  --debug            enable debug information
  --verbose          makes generator more verbose
  --threads THREADS  number of threads to run simultaneously
  --test             run a scenario only once
```

## Authors / Contributors

* [Samuel Vandamme](http://www.sava.be)
* Stijn Polfliet
<img src="http://docs.coscale.com/gfx/logo.png" alt="CoScale logo" />
