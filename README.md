# Center for Open Science JavaScript Style

> JavaScript Style based on [AirBnB's JavaScript Guide](https://github.com/airbnb/javascript)

[![npm version](https://badge.fury.io/js/%40centerforopenscience%2Feslint-config.svg)](https://badge.fury.io/js/%40centerforopenscience%2Feslint-config)
[![Build Status](https://travis-ci.org/CenterForOpenScience/javascript.svg?branch=master)](https://travis-ci.org/CenterForOpenScience/javascript)

* For vanilla JavaScript projects, use @centerforopenscience/eslint-config (or just @centerforopenscience, eslint will append /eslint-config automatically)
* For Ember Applications, use @centerforopenscience/eslint-config/ember

# @centerforopenscience/eslint-config

> Generic ESLint configuration for the Center for Open Science

Based on [AirBnB's JavaScript Guide](https://github.com/airbnb/javascript), with a few notable exceptions including:

* Indentation of 4 spaces instead of 2
* Allow `for..of` loops
* Allow `++`
* Turn off some import rules and make others warnings
* `max-len` is a warning, until we get the various repos cleaned up
