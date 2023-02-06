---
title: Fixing authentication issues
---

## ERR_CLEARTEXT_NOT_PERMITTED

This is a bug in older Android versions of Kaiteki where the website redirected you to the local web server Kaiteki is running, which does not support HTTPS. 

If you are affected by this, you can open the URL listed in the error message in a browser, in order to complete the login process.