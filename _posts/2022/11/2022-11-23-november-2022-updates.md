---
title: "November 2022 Updates"
layout: post
author: craftplacer
banner: "/img/november-2022-updates/thumbnail.png"
---

Between October and November, focus was laid on bringing essential features to the table.

## Notifications

![The new notifications screen as seen in Kaiteki, with read and unread tabs and a 'mark all as read' button]({% link img/november-2022-updates/notifications.jpg%})

A basic feature finally joined in, we now have functioning notifications.

It's not feature complete quite yet, you can check out [![issue 56](https://img.shields.io/github/issues/detail/state/Kaiteki-Fedi/Kaiteki/56)](https://github.com/Kaiteki-Fedi/Kaiteki/issues/56) for more details.

## Emoji picker and reactions

![The new emoji picker with tabs and a search bar]({% link img/november-2022-updates/emoji-picker.png %})

A proper emoji picker is now available. It also supports Unicode emojis, in order to support reactions.


## Experimental Twitter Support

Kaiteki now has support for Twitter, although still has many [flaws]({% link compatibility.html %}#twitter).

<video controls muted>
    <source src="{% link vid/A9C81CCB.webm %}" type="video/webm">
</video>

## Attachment changes

### Better alt text support

<img src="{% link img/1D6BBD67.png %}">

You can properly view the alt text of attachments now. Previously they were displayed in the AppBar, but that was very unfriendly for reading descriptive alt text.

## Minor changes

- Fixed `ERR_CLEARTEXT_NOT_PERMITTED` for Android versions