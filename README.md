# ext-check

> Check and fix extensions before importing into Qlik Sense Server.

![](http://serve.mod.bz/branch/)

## About

## Prerequisites

Node.js + NPM installed on your system.

## Install

Install the tool globally.

```npm install ext-check -g
```
## Run

Run `ext-check` in the command line using one of the following options:

### Just check

Just check the visualization extension, the output in the command line will indicate if there is a problem which needs to be fixed.

ext-check "myExtension.zip"

### Check and fix

Checks the extension, fixes potential problems in the source zip-file (create a backup with %filename%.bak before) immediately.

```ext-check "myExtension.zip" --fix
```
### Check and fix, no backup

```ext-check "myExtension.zip" --fix --backup=false
```
### Check using a password protected zip file

```ext-check "myExtension.zip" --password "verysecurepwd"
```
## Options

* **`--help`** (alias `-h`) - Show the help
* **`--fix`** (alias `-f`) - Whether to fix the file or not (defaults to `false`)
* **`--backup`** (alias `-b`) - Whether to create a backup or not (defaults to `true`)
* **`--password`** (alias `-p`) - Password for the zip-file (if applicable)

## Author

**Stefan Walther**

+ [qliksite.io](http://qliksite.io)
* [twitter/waltherstefan](http://twitter.com/waltherstefan)
* [github.com/stefanwalther](http://github.com/stefanwalther)

## License

Released under the MIT license.

***

_This file was generated by [verb-cli](https://github.com/assemble/verb-cli) on September 18, 2015._