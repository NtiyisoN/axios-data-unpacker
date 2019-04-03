# Axios Data Unpacker

Axios middleware that unpacks HTTP responses so that you can focus on actual response

[![Build Status](https://travis-ci.org/anubhavsrivastava/axios-data-unpacker.svg?branch=master)](https://travis-ci.org/anubhavsrivastava/axios-data-unpacker)
[![Coverage Status](https://coveralls.io/repos/github/anubhavsrivastava/axios-data-unpacker/badge.svg?branch=master)](https://coveralls.io/github/anubhavsrivastava/axios-data-unpacker?branch=master)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
[![GitHub issues](https://img.shields.io/github/issues/anubhavsrivastava/axios-data-unpacker.svg?style=flat-square)](https://github.com/anubhavsrivastava/axios-data-unpacker/issues)

[![NPM](https://nodei.co/npm/axios-data-unpacker.png?downloads=true&stars=true)](https://nodei.co/npm/axios-data-unpacker/)

---

## Introduction

Axios data unpacker is middleware for axios that unpacks `data` from axios standard response and makes API response content to called so that one can focus on actual response.

### The Problem

Any HTTP request using axios will return into following object that is available to callee function,

    {
        // `data` is the response that was provided by the server
        data: {},

        // `status` is the HTTP status code from the server response
        status: 200,

        // `statusText` is the HTTP status message from the server response
        statusText: 'OK',

        // `headers` the headers that the server responded with
        headers: {},

        // `config` is the config that was provided to `axios` for the request
        config: {}
        }

This would imply that application has to unpack `data` object at all places of consumption something like,

    getUsers() {
        return axios.get('/users').then( function (result) {
            return result.data;
        });
    }

---

## Install

---

## Usage

### Node usage

### Browser

### Configuration

### Advanced Usage

---

<!-- References
https://laracasts.com/discuss/channels/servers/get-data-out-from-axios-javascript -->

## Contribution

Suggestions and PRs are welcome!

Please read the [contribution guidelines](CONTRIBUTING.md) to get started.

<!-- Change contributing.md -->

---

## License

[![Open Source Love](https://badges.frapsoft.com/os/mit/mit.svg?v=102)](LICENSE)

refer `LICENSE` file in this repository.

---
