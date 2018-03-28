## Preamble

    GIP: <to be assigned>
    Title: Browser extension with Bounties universe
    Author: Fred Lin
    Type: Standard Track
    Category Interface
    Status: Draft
    Created: 2018-03-28

## Simple Summary

Integrate [Bounties universe](https://gitcoin.co/universe) into [Gitcoin web extension](https://github.com/gitcoinco/chrome_ext/) and provide UI to filter bounties.

## Abstract

Update bounties api to support Bounties universe, add essential UI to filter bounties from multiple sources.

## Motivation

[Gitcoin web extension](https://github.com/gitcoinco/chrome_ext) provides an enhanced experience of [Gitcoin Bounties explorer](https://gitcoin.co/explorer)
 when browsing bounties in github.

The main enhancements are:

* quickly browse available bounties in popup
* browse funded work directly on github
* filter available work from github
* fund work directly on github
* tip user directly on github

Besides Gitcoin Bounties, the new [Bounties universe](https://gitcoin.co/universe) provide ethereum related bounties around internet.

We can integrate data by updating existing API and provide a convenient extension to:

* quickly browse available bounties from Gitcoin Bounties explorer and Bounties universe in popup
* browse all funded work directly on github

By adding essential UI in browser extension, user could filter bounties from multiple sources.

All developer seeking for bounties could install the extension and find best fit from all available sources.
When they adapt to use the extension, Gitcoin bounty is the most convenient option when they want to tip or fund a new bounty.

## Specification

Based on https://github.com/gitcoinco/web/blob/master/docs/API.md#bounties

The Proposed API (version 0.2) add the `source` field key to indicate where the bounty funded.

| Field Key | Datatype | Description | Default value |
|---------|--------|--------------------------------| --------|
| source | string | where the bounty funded | gitcoin |

Possible value: all, gitcoin, openbounty, hackerone,bounty0x

Example:

```
https://gitcoin.co/api/v0.1/bounties/?idx_status=open&network=mainnet&source=all&order_by=-web3_created
```

## Rationale


## Backwards Compatibility

The default `source` field key will be `gitcoin`, which is compatible with current (version 0.1) API.

## Implementation
The implementations must be completed before any GIP is given status "Final", but it need not be completed before the GIP is accepted. While there is merit to the approach of reaching consensus on the specification and rationale before writing code, the principle of "rough consensus and running code" is still useful when it comes to resolving many discussions of API details.

## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
