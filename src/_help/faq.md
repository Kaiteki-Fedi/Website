---
title: Frequently asked questions
---

## What is Kaiteki?

In old man terms, Kaiteki is the following:

> A cross-platform client for micro-blogging services

Kaiteki is designed to work with websites similar to Twitter. The cross-platform part has a factor of two, because it supports multiple services (Mastodon-based, Misskey, Twitter, and whatever you can add support for) as well as multiple devices and operating systems (thanks to Flutter).

### Goals

Kaiteki tries to be powerful yet user-friendly.

Kaiteki follows the cutting-edge [Material Design guidelines from Google](https://material.io/) in order to deliver a high quality user experience.

You are open to send us feedback and we will try to honor it.

## What is Kaiteki **not**?

### A client tailored to just one platform

Kaiteki started out with Pleroma in mind, but as it started off, the goal quickly switched to interoperability with Mastodon and Misskey. While doing so, Kaiteki has to be platform-agnostic and has to adapt in all kinds of situations.

### A Web-based client

Kaiteki won't be truly native (as it's on top of Flutter and Dart), but it doesn't use Electron (nor Chromium) to handle it's UI. With Flutter growing and evolving there are many improvements to be seen that Kaiteki will inherit and benefit from.

### Fedilab and Fedi.app

While both apps and Kaiteki share many features and intentions, there are giant philosophical differences in how things are handled.

Kaiteki is trying to be traditional, yet flexible and modern.

### An ActivityPub client

ActivityPub is a server protocol. This means, that it enables instances running Mastodon, Pleroma, Misskey and so on to communicate and federate with each other.

Kaiteki only interfaces to the APIs of the services that it supports and is not capable of doing federation on its own. Kaiteki is also not limited to just Fediverse backends.