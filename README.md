# CMU-Q Client Services - static assets

Static images used by CMU-Q Client Services workflows on managed Macs (for example the app icons shown in
install prompts). Files are served with GitHub Pages:

    https://cmuq-client-services.github.io/assets/icons/<name>.png

## Layout
- `icons/` - application icons, PNG, named after the Installomator label of the app (for example `firefoxpkg.png`, `visualstudiocode.png`).
  Apps that Installomator has no label for (macOS system apps, in-house tools) use a lowercase-hyphen name. A `-2021` suffix marks an older artwork version.
- `setup-manager/` - banners, app icons and instruction screenshots used by the Jamf Setup Manager / Setup Checklist configuration.
- `branding/` - CMU-Q logo.
- `pkgs/` - installer packages that must be downloadable WITHOUT authentication by a Mac during Automated Device Enrollment (currently only the
  Jamf Setup Manager package, Developer ID signed and notarized by Jamf; sha256 e0df46d5...9e9b for 1.4.7-652). Jamf Pro serves a manifest that points here.
- `wallpapers/` - desktop wallpapers for managed Macs (`cmuq-wallpaper-<black|tartan|grey|red>-3840x2160.jpg`): tartan background with the
  stacked CMU-Q wordmark, 3840x2160 (16:9), JPEG quality 85, 4:4:4. The wordmark sits in the left third, so the picture is safe to crop to
  16:10 and 3:2 MacBook screens; Macs fill the screen, so no other sizes are needed.

## Notes
- All product names, logos and icons belong to their respective owners and are used here only to identify the
  software being installed on CMU-Q managed devices.
- Nothing in this repository is secret. Do not add credentials, tokens, internal hostnames or installers (the only exception is `pkgs/`, see above).
- Changes go through a pull request reviewed by a second person. Do not rename or delete files that managed
  devices may still request without checking first.

Maintained by CMU-Q Client Services.
