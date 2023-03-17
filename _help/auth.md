---
title: Issues while signing-in
---

Authentication is a complex subject and many bugs can occur while doing so. Here below you see already known issues and potential workarounds.

## ERR_CLEARTEXT_NOT_PERMITTED

This is a bug in older Android versions of Kaiteki where the website redirected you to the local web server Kaiteki is running, which does not support HTTPS. 

If you are affected by this, you can open the URL listed in the error message in a browser, in order to complete the login process.

## Stuck at "Authentication Successful"

Kaiteki's dependency [`url_launcher`](https://pub.dev/packages/url_launcher) launches URLs in a WebView without controls by default. To circumvent this softlock close and reopen the app again, which should leave you signed in this time.