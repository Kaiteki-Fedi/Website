---
title: "Major quality release"
layout: post
author: craftplacer
banner: "/img/major-quality-release/thumbnail.png"
---

This new commit batch had many code fixes this time, resulting in less broken elements making Kaiteki more usable.

## UI changes

- The main screen has a compact navigation rail now with the compose button being permanently visible.

- Slight compose dialog redesigns, alongside it being the first dialog to be adaptive to the screen resolution.

  (Try resizing your window while having it open!)

- Post metadata should now have the correct color for the current theme.

## Bug fixes

- Debug post submission has been removed. This slipped into production making it impossible to actually submit posts via Kaiteki.

- Rich text will now inherit from the surrounding UI. Expect less black or white text contrasting out of nowhere.

- Emojis are now 1.5x of the normal text height, making them more readable.

- The login screen now got its transition animation.

- Kaiteki will display a placeholder avatar when the remote image is not accessible.

## Code quality changes

- ApiToDart has been worked on, ensuring more accurate generation of data classes, Misskey being the one benefiting most out of it.

- The data of API responses are now being saved in another class, to ensure being able to correctly parse error messages in case of any. This also resolves Kaiteki being unable to parse errors from Misskey.

- More default values and fallbacks for Misskey data model conversion.

and many more minor changes...