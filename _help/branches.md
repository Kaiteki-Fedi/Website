---
title: Branches & flavors
---

Kaiteki is compiled by hand or compiled automatically, and potentially distributed to a store. Kaiteki can also be built with or without proprietary code. This page will explain the different flavors Kaiteki has.

## Stable vs. Nightly

Stable builds are made in weekly increments in order to ensure quality and stability. Nightly builds are produced on every code change made by the developers in order to provide feature previews and to find issues early.

## FOSS vs. Store

Kaiteki will be distributed to different software marketplaces such as Google Play, App Store or the Microsoft Store. Kaiteki's "store flavor" will contain support for proprietary services like [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging) (push notifications powered by <abbr title="Google Mobile Services">GMS</abbr>) or Tenor.

Kaiteki's FOSS version has no support for these services and provides alternatives such as [UnifiedPush](https://unifiedpush.org/).

## Signed vs. Unsigned

Security is required by mobile operating systems, such as Android. Builds are signed as to ensure that they are made only by the development team.

Not everyone has or should have access to the certificates and keys used to sign Kaiteki, thus by default Kaiteki is built *unsigned*. Unsigned builds have the suffix `.dev` added to the package ID to avoid conflict with the production/stable version of Kaiteki.

On Android, packages with the same ID but different signature are reported as invalid and can't be updated.