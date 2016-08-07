# chrome-extension-skeleton

[![No Maintenance Intended](http://unmaintained.tech/badge.svg)](http://unmaintained.tech/)

A skeleton application which can be used to create new Google Chrome extensions.

## Installation

Simply run `npm install` and next `grunt` to create the extension. The extension will be 
created in *build/packed/*

## Configuration

The name in `package.json` is used as the name of your extension. A `<name>.crx` file will be generated
in *build/packed/* together with a `<name>.zip` file. In order to create the *.crx* file, a private key
should be stored in `resources/<name>.key`. When no key is present, the key will automatically be generated.

A chrome extension contains a `manifest.json` file. This file is stored in the resources directory and can be
adjusted at will. Note that the file does not contain a `name` and `version` property since they will be added
dynamically by Grunt. The name and version are taken from the package.json.

## Documentation

* https://developer.chrome.com/extensions
* https://developer.chrome.com/extensions/devguide
