# Youtube-Music---Spotube-plugin
Initial Release

What's included

- Custom YouTube Music plugin for Spotube.
- Packaged ".smplugin" file for download.

Notes

- This is the initial public release.
- Working Spotube version 5.1.2

Changelog
2.0 — 2026-10-25

Changed

Renamed the plugin from YouTube Music Google Login to YouTube Music.
Removed Google sign-in wording from the manifest description.
Bumped the version to 2.0.
Notes
Manifest-only release: plugin.out is byte-identical to 1.2.1 and 1.2.2.
The plugin slug changes from youtube-music-google-login to youtube-music, so the stored session is not reused. Sign in again after installing.
Uninstall older builds first. An old plugin with the same name (YouTube Music 1.0.x) is rejected as a duplicate.

1.2.2 — 2026-10-25

Added
repository field to the manifest, enabling the version badge in Spotube.

Security
Added a single HTTP request sink with strict URL validation: HTTPS-only music.youtube.com, allowed endpoint paths, no userinfo, no query or fragment, and no encoded path tricks.

Disabled redirects at the HTTP layer and reject 3xx responses.

Added a cookie allowlist and filtering; only required YouTube Music cookies are stored.

Centralized session application and auth hashing per request.

Changed
Improved sign-in failure guidance for the in-app Google flow and the Cookie fallback.

- Important Note: 
This is not the final version of the plugin. To prevent potential issues and ensure continued improvements, it will be updated over time. To avoid misleading users, please note that the code was written entirely by AI. The plugin is currently working correctly and is being tested by other users.

- Plugin is NOT official release from Google or Youtube
