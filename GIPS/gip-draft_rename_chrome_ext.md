## Preamble

    GIP: <to be assigned>
    Title: Rename chrome_ext to gitcoin-extension
    Author: Fred Lin
    Type: Standard Track
    Category Core
    Status: Draft
    Created: 2018-03-31

## Simple Summary

Rename the repo https://github.com/gitcoinco/chrome_ext/ .

## Abstract

Rename `gitcoinco/chrome_ext` to `gitcoinco/gitcoin-extension` to reflect the repo's purpose.

## Motivation

`gitcoinco/chrome_ext` hosts gitcoin browser extension for Chrome and now plan to support more browsers. The repo name could be changed to reflect the purpose.

## Specification

* Rename repo `gitcoinco/chrome_ext` to `gitcoinco/gitcoin-extension` on [github](https://github.com/gitcoinco/chrome_ext/settings).
* Change `manifest.json` or `package.json` to reflect the new repo location.

## Rationale

* [Thread](https://github.com/gitcoinco/chrome_ext/issues/47#issuecomment-373538801) to discuss about renaming to `web_ext`.
* [MetaMask extension](https://github.com/MetaMask/metamask-extension) use `metamask-extension` as its repo name.
* [Provide Firefox version of Gitcoin Chrome Extension](https://github.com/gitcoinco/chrome_ext/issues/1)

## Backwards Compatibility

None.

## Test Cases

Not inflect the end user.

## Implementation

Change the project name.

## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
