---
title: Privacy Policy
permalink: /advanced-scene-switcher/privacy
---

# Privacy Policy

Effective date: 2026-11-10

This policy describes how the Advanced Scene Switcher plugin for OBS Studio
handles data when you use its YouTube features.

## YouTube API Services

The plugin uses YouTube API Services. By using its YouTube features you agree
to the [YouTube Terms of Service](https://www.youtube.com/t/terms). See also
the [Google Privacy Policy](https://policies.google.com/privacy).

The YouTube features are optional. They are only active after you connect a
YouTube account in the plugin.

## Requested permission

The plugin requests the OAuth scope
`https://www.googleapis.com/auth/youtube` ("Manage your YouTube account").

## Data the plugin accesses

The plugin accesses the following data via the YouTube Data API, only for the
features you configure:

- The channel ID and channel name of the connected account.
- Your live broadcasts (title, description, status, scheduled start time,
  settings) and live streams (stream key association, stream health).
- The list of YouTube video categories.

## Data the plugin sends to YouTube

Only when you configure a macro to do so, the plugin:

- Creates, starts and ends live broadcasts with the title, description,
  privacy, category and other settings you entered.
- Uploads a thumbnail image file you selected.

## Storage

- All data is stored only locally on your computer, as part of the OBS scene
  collection files. This includes the OAuth refresh token, the channel ID and
  name, and, if you use your own Google Cloud project, your OAuth client ID
  and secret.
- Short-lived access tokens and API responses are only kept in memory while
  OBS is running. Responses are cached for at most 30 seconds.
- Exported macros do not contain the client secret or the refresh token. The
  plugin's full settings export does contain them, so treat that file as
  private.

## Sharing

- The developer does not operate any server and does not receive any user
  data. All requests go directly from your computer to Google.
- No data is shared with third parties, sold, or used for advertising or
  analytics.
- During sign-in the plugin briefly runs a local web server on 127.0.0.1 to
  receive the authorization from your browser. It is not reachable from other
  computers and stops once sign-in is complete or after 120 seconds.

## Revoking access and deleting data

- Removing the YouTube connection in the plugin revokes the plugin's access
  and removes the stored data for it.
- You can also revoke access at any time at
  <https://security.google.com/settings/security/permissions>.
- Uninstalling the plugin or deleting the OBS scene collection removes all
  locally stored data.

## Contact

<https://github.com/WarmUpTill/SceneSwitcher/issues>
