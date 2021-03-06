---
title: Addr v2

## Optional.  An entry will be added to the topics index for each alias
#aliases:
#  - Foo

## Required.  At least one category to which this topic belongs.  See
## schema for options
categories:
  - P2P Network Protocol

## Required.  Use Markdown formatting.  Only one paragraph.  No links allowed.
## Should be less than 500 characters
excerpt: >
  **addr v2** is a proposed new version of the `addr` message in the
  Bitcoin P2P network protocol, which is used to advertise the addresses
  of nodes that accept incoming connections.

## Optional.  Use Markdown formatting.  Multiple paragraphs.  Links allowed.
extended_summary: |
  The original `addr` message allows relaying 128-bit IPv6 addresses
  with backwards compatibility for IPv4 and [onioncat-encoded][] version
  2 (v2) Tor hidden service (.onion) addresses.  However, v3 Tor hidden
  service addresses are 256 bits in size, as are addresses for several
  other privacy-enhancing network protocols.  Since those newer address
  types can't be used with the existing `addr` message, a new version of
  the message has been proposed.  Additionally, the update may allow
  tweaking other aspects of the message or the behavior of nodes and
  clients that process it.

  [onioncat-encoded]: https://web.archive.org/web/20121122003543/http://www.cypherpunk.at/onioncat/wiki/OnionCat

## Optional.  Produces a Markdown link with either "[title][]" or
## "[title](link)"
primary_sources:
    - title: BIP155

## Optional.  Each entry requires "title", "url", and "date".  May also use "feature:
## true" to bold entry
optech_mentions:
  - title: Version 2 `addr` message proposed
    url: /en/newsletters/2019/03/12/#version-2-addr-message-proposed
    date: 2019-03-12

  - title: Version 2 `addr` message assigned BIP155
    url: /en/newsletters/2019/07/31/#bips-766
    date: 2019-07-31

  - title: Proposed per-node signaling for address relay with v2 `addr` messages
    url: /en/newsletters/2019/11/06/#signaling-support-for-address-relay
    date: 2019-11-06

## Optional.  Same format as "primary_sources" above
see_also:
  - title: P2P protocol `addr` message
    link: https://btcinformation.org/en/developer-reference#addr
---
