# Platform Overview

## About
This document details the overall structure of the Buttercup platform, the projects and how they interact.

## Top-Down Dependencies
The following list details the higher-level components and their nested dependencies:

 * [Buttercup Desktop](https://github.com/buttercup/buttercup-desktop) - Desktop application for accessing Buttercup vaults
   * [Buttercup Core](https://github.com/buttercup/buttercup-core) - Core library for Vault manipulation and reading
     * [Datasources](https://github.com/buttercup/datasources) - Vault datasource implementations (Dropbox/ownCloud etc.)
     * [Credentials](https://github.com/buttercup/credentials) - Key implementation for unlocking things (vaults, etc.)
 * [Buttercup Mobile](https://github.com/buttercup/buttercup-mobile) - Mobile app for accessing Buttercup vaults
   * Buttercup Core
     * ...
   * [Buttercup Crypto](https://github.com/buttercup/crypto) (Rust base - used in mobile only) - Cryptographic tools for cross-platform use
 * [Buttercup Browser Extension](https://github.com/buttercup/buttercup-browser-extension) - Browser extension for major browsers
 
### Buttercup Core
The core library makes use of toolkits like **Datasources** and **Credentials**.

Datasources contains implementations for all the major vault sources, like Dropbox, for instance. Datasources contains its own implementation for network requests and encryption (crypto is performed in Datasources).

Credentials is a toolkit for creating and reading encrypted short-strings, used for storing login details to Datasources and other endpoints or vaults. Encryption is also performed in this library.
