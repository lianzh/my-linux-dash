# Linux Dash

A simple, low-overhead web dashboard for GNU / Linux. (~1MB)

[**DEMO**](http://linuxdash.afaqtariq.com) | [**Installation Instructions**](#installation)

![Linux Dash screenshot](https://raw.githubusercontent.com/afaqurk/screenshots/master/linux-dash/system-status-full.png)

## Features
* A beautiful, simple web-based dashboard for monitoring a linux server
* Only 1MB on disk! (.git removed)
* Live graphs, refresh-able widgets, and a growing # of supported modules
* Drop-in install for PHP (Apache, NGINX) and Node.js 

## Installation

### PHP
 
1. Make sure you have the `exec`, `shell_exec`, and `escapeshellarg` functions enabled
2. Go to the web root for your server 
  - `/var/www/` by default for Apache
  - For help with nginx setup, see [this gist](https://gist.github.com/sergeifilippov/8909839) by [@sergeifilippov](https://github.com/sergeifilippov).
3. Get a copy of Linux Dash by one of the following methods:
  - Use composer, run `composer create-project afaqurk/linux-dash -s dev`
  - Or clone the git repo: `git clone https://github.com/afaqurk/linux-dash.git`
  - Or [download the source](https://github.com/afaqurk/linux-dash/archive/master.zip)

### Node.js

1. Get a copy of Linux Dash by one of the following methods
  - Clone the git repo: `git clone https://github.com/afaqurk/linux-dash.git`
  - Or [download the source](https://github.com/afaqurk/linux-dash/archive/master.zip)
2. Go into the linux-dash folder and run `npm install`
3. Start Linux Dash by running: `node server`

## Security

**Please note: If you would like to limit access to linux-dash, please add
`.htaccess` or other security measure.**

## Goals for v2.0
- [x] Backend ported to ~~ Python ~~ shell scripts & python from PHP
- [x] Add config file
- [x] Segregate core code-base and modules
- [ ] Each module in a separate directory with front-end template, back-end file, bash script
- Add project to package managers
  - [x] npm
  - [x] composer
  - [ ] aur
  - [ ] apt
- [x] Bonus: multiple server side languages supported
  - node & php currently

## Support
* OS
    * Arch
    * Debian 6, 7
    * Ubuntu 11.04+
    * Linux Mint 16+
    * CentOS 5, 6
* Apache 2
* Nginx
* PHP 5
* Modern browsers
