# Center for Open Science JavaScript Style

> JavaScript Style based on [AirBnB's JavaScript Guide](https://github.com/airbnb/javascript)

[![npm version](https://badge.fury.io/js/%40centerforopenscience%2Feslint-config.svg)](https://badge.fury.io/js/%40centerforopenscience%2Feslint-config)
[![Build Status](https://travis-ci.org/CenterForOpenScience/javascript.svg?branch=master)](https://travis-ci.org/CenterForOpenScience/javascript)

* For vanilla JavaScript projects, use [@centerforopenscience/eslint-config](#centerforopenscienceeslint-config)
* For Ember Applications, use [@centerforopenscience/eslint-config/ember](#centerforopenscienceeslint-configember)

## @centerforopenscience/eslint-config

> Generic ESLint configuration for the Center for Open Science

Based on [AirBnB's JavaScript Guide](https://github.com/airbnb/javascript), with a few notable exceptions including:

* Indentation of 4 spaces instead of 2
* Allow `for..of` loops
* Allow `++`
* Turn off some import rules and make others warnings
* `max-len` is a warning, until we get the various repos cleaned up

#### Usage

Add the following to your ESLint config file:
```javascript
{
    "extends": "@centerforopenscience"
}
```
Note: ESLint automatically appends /eslint-config so it is not necessary to add it here.

## @centerforopenscience/eslint-config/ember

> Ember ESLint configuration for the Center for Open Science

Based on [COS's Base Config](https://github.com/CenterForOpenScience/javascript/blob/master/index.js) with [eslint-plugin-ember](https://github.com/netguru/eslint-plugin-ember)

Since route-able components aren't stable, this is unnecessary:
* `alias-model-in-controller`

This will produce too many errors or warnings to count, so for now, it's turned completely off:
* `use-ember-get-and-set`

The following are set to warnings, but will become errors later:
* `no-observers`
* `no-function-prototype-extensions`
* `named-functions-in-promises`
* `order-in-components`
* `order-in-routes`
* `order-in-controllers`

#### Usage

Add the following to your ESLint config file:
```javascript
{
    "extends": "@centerforopenscience/eslint-config/ember"
}
```
Note: You must include /eslint-config in the path for non-default configurations.
