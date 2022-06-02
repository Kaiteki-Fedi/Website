---
title: "Login experience overhaul"
layout: post
author: craftplacer
---

With commit [`29656d1`](https://github.com/Craftplacer/Kaiteki/commit/29656d1a9c95076acce269610ac71be8ff23cd88) the entire login screen was revamped.

<video controls muted>
    <source src="{{site.url}}/vid/30EEC26950A328CA.mp4" type="video/mp4">
    <source src="{{site.url}}/vid/3167C3AB3499549B.webm" type="video/webm">
</video>

## New features

- **Instance probing:** No need for knowing what software your instance runs on. Kaiteki will send out requests to known endpoints and will check what kind of instance you have.
- **Animations.** (some of them are borked)
- **List of "suggested" instances** for Fediverse newcomers, alongside a short description of most instances alongside their rules. (available here) 
- Instance logo and background are visible at the login screen
- *Lots of necessary internal changes*

## Recent changes since first announcement

- First implementation of keyboard shortcuts, more coming soon
- About screen design changes (now shows Kaiteki’s colorful logo)
- Tooltips on post scope and time (should also aid in screen readers)
- Post time is displayed properly now (If conditions were messed up)

You can try these changes now at: [kaiteki.craftplacer.moe](https://kaiteki.craftplacer.moe/)