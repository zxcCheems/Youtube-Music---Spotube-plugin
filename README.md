# YouTube Music — Spotube Plugin

- A community-made YouTube Music plugin for Spotube.

# Initial Release

# What's Included

- Custom YouTube Music plugin for Spotube.

- Packaged .smplugin file available for download.

# Requirements

- Spotube version 5.1.2.

# Changelog

# 2.0 — 2026-10-25

# Changed

- Renamed the plugin from YouTube Music Google Login to YouTube Music.

- Removed Google sign-in wording from the manifest description.

- Updated the plugin version to 2.0.

# Important Notes

- This is a manifest-only release. The plugin.out file is byte-identical to versions 1.2.1 and 1.2.2.

- The plugin identifier changed from youtube-music-google-login to youtube-music. As a result, the previous stored session will not be reused, and you will need to sign in again.

- Uninstall older builds before installing this version.

- Spotube may reject this plugin as a duplicate if an older YouTube Music 1.0.x plugin is already installed.

# 1.2.2 — 2026-10-25

# Added

- Added the repository field to the manifest to enable the version badge in Spotube.

# Security

- Added a single HTTP request sink with strict URL validation: HTTPS-only requests to music.youtube.com, allowed endpoint paths, no userinfo, no query strings or fragments, and no encoded path tricks.

- Disabled HTTP redirects and added rejection of 3xx responses.

- Added cookie allowlisting and filtering so that only required YouTube Music cookies are stored.

- Centralized session application and per-request authentication hashing.

# Improved

- Improved sign-in failure guidance for the in-app Google sign-in flow and the cookie fallback method.

- Important Notice

- This is an experimental project and not the final version of the plugin. Updates may be released to fix bugs, improve stability, and address compatibility issues.

- The code was written entirely by AI and is being tested by users. Although the plugin is currently working as expected, bugs or unexpected issues may occur.

If you encounter any problems, please report them so they can be investigated and addressed in future updates.

Disclaimer: This is an unofficial community project. It is not affiliated with, endorsed by, or supported by Google, YouTube, or Spotube. Use it at your own discretion.
