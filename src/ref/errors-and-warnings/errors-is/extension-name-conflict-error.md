---
summary: Resolve the Extension Name Conflict Error in OutSystems 11 (O11) by renaming the duplicate extension in Integration Studio.
locale: en-us
guid: b888bd38-658f-4d8d-b3c7-df225c1330b0
app_type: traditional web apps, mobile apps, reactive web apps
platform-version: o11
figma:
tags: error handling, extension management, platform server, integration studio, publishing apps
audience:
  - mobile developers
  - frontend developers
  - full stack developers
outsystems-tools:
  - integration studio
  - service studio
coverage-type:
  - unblock
---

# Extension Name Conflict Error

Message
:   `Extension Name <name> already exists. Please rename it in Integration Studio before trying to store or publish it again.`

Cause
:   There is another extension with the same name in the Platform Server you are connected to.

Recommendation
:   You must change the [extension name](<../../integration-studio/element-property/extension.md>).
