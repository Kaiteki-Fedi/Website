---
layout: default
title: Development Notes
include-title: true
---

<h2>Kaiteki's API structure</h2>

<figure>
    <img src="{% link img/api-structure.png %}" width="600" style="display: block; margin: 0 auto; max-width: 100%;">
    <figcaption>Kaiteki's internal code structure, starting from the frontend all the way to the backends</figcaption>
</figure>

To make Kaiteki <abbr title="compatible with any backend">backend-agnostic</abbr>, it is important to make the app not reliant on any feature or data structure imposed by a certain API. While we don't know what best practice is, there are open doors to keep iterating on the internal parts of the app on how things are implemented.

Let's talk about how Kaiteki is built up:

1. Here we have **Kaiteki** itself. [Kaiteki defines it's own data structures](https://github.com/Kaiteki-Fedi/Kaiteki/tree/master/src/kaiteki/lib/fediverse/model) used throughout the application.

2. We use the [**adapter** design pattern](https://refactoring.guru/design-patterns/adapter), we define basic capabilities that a social media backend can perform. [We also use mixins (i.e. interfaces)](https://github.com/Kaiteki-Fedi/Kaiteki/tree/master/src/kaiteki/lib/fediverse/interfaces), to implement individual features not shared by every backend. Currently adapters differentiate whether they support *chatting* or *reactions* (both not supported by Mastodon).

3. We create **client** classes which correspond to API endpoints. A key principle from Kaiteki is to not tamper with the API endpoints or models. This is why adapters exist.

4. At the end all requests go to the **APIs** themselves.