---
title: "Windows"
description: "Resources for passkeys in Microsoft Windows"
date: 2022-09-03T16:09:38.358Z
draft: false
images: []
menu:
  docs:
    parent: "reference"
weight: 1005
toc: true
---

{{% ds-la_p-ea_s %}}

## Overview

Windows Hello, the local platform authenticator in Windows 10 and 11, has the following capabilities:

- creating and using [***device-bound*** passkeys](../terms#device-bound-passkey) on the local device
- creating and using [***device-bound*** passkeys](../terms#device-bound-passkey) on a FIDO2 security key

The following is also possible in Windows 11 version 23H2 and newer:

- using passkeys from iOS and iPadOS devices for signing into services in all browser and native apps using [FIDO Cross-Device Authentication](../terms#cross-device-authentication-cda)
- using passkeys from Android devices for signing into services in all browser and native apps using [FIDO Cross-Device Authentication](../terms#cross-device-authentication-cda)

The following is also possible in both Windows 10 and Windows 11 (earlier than 23H2):

- using passkeys from iOS and iPadOS devices in Chrome (108+) and Edge (108+) for signing in to web services using [FIDO Cross-Device Authentication](../terms#cross-device-authentication-cda)
- using passkeys from Android devices in Chrome (108+) and Edge (108+) for signing in to web services using [FIDO Cross-Device Authentication](../terms#cross-device-authentication-cda)

## Platform Notes

- The [authenticatorAttachment property of responses](https://w3c.github.io/webauthn/#dom-publickeycredential-authenticatorattachment), planned for specification delivery in WebAuthn L3, is not currently available in responses to `navigator.credentials.get` when using the platform authenticator or a hardware security key. It is supplied during credential creation, or when using [FIDO Cross-Device Authentication](/docs/reference/terms/#cross-device-authentication-cda) for an authentication ceremony.

### Cross-Device Authentication

Starting in Windows 11 version 23H2, [FIDO Cross-Device Authentication (CDA)](../terms#cross-device-authentication-cda) is supported globally at the operating system level and available for all apps and browsers. Persistent linking is available between Android devices (authenticator) and Windows 11 23H2+. iOS and iPadOS do not support persistent linking.

In Windows versions prior to 11 23H2, including Windows 10, support for [FIDO Cross-Device Authentication (CDA)](../terms#cross-device-authentication-cda) is only available in Chrome and Edge. It is not available globally. Persistent linking is available between Android devices (authenticator) and Chrome and Edge (clients) on these versions. iOS and iPadOS do not support persistent linking.

## Resources

> Coming Soon
