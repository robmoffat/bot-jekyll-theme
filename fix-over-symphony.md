---
layout: post
title: FIX over Symphony
description: Sending FIX (Financial Exchange) Messages via the Symphony Platform
image: assets/images/fixprotocol.png
menu: true
---

Do you want to send FIX messages via Symphony?  We have a library for that!  Built by Rob Moffat for Deutsche Bank and then Open-Sourced as part of their Symphony tools project, this integration allows you to encode FIX messages into JSON, using the popular QuickFix and Jackson libraries.

## [QuickFIX/JSON Project](https://github.com/robmoffat/symphony-java-client-parent/tree/master/quickfix-json)

Note, this doesn't _need_ Symphony, but Symphony is an _ideal_ transport for FIX messages in JSON format!  Why come up with your own in-house, incompatible, inconsistent data formats when they have _already been standardized many years ago_?

