# CMU-Q Client Services - static assets

Static images used by CMU-Q Client Services workflows on managed Macs (for example the app icons shown in
install prompts). Files are served with GitHub Pages:

    https://cmuq-client-services.github.io/assets/icons/<name>.png

## Layout
- `icons/` - application icons, PNG, named after the Installomator label of the app (for example `firefoxpkg.png`, `visualstudiocode.png`).
  Apps that Installomator has no label for (macOS system apps, in-house tools) use a lowercase-hyphen name. A `-2021` suffix marks an older artwork version.
- `setup-manager/` - banners, app icons and instruction screenshots used by the Jamf Setup Manager / Setup Checklist configuration.
- `branding/` - CMU-Q logo.

## Notes
- All product names, logos and icons belong to their respective owners and are used here only to identify the
  software being installed on CMU-Q managed devices.
- Nothing in this repository is secret. Do not add credentials, tokens, installers or internal hostnames.
- Changes go through a pull request reviewed by a second person. Do not rename or delete files that managed
  devices may still request without checking first.

Maintained by CMU-Q Client Services.
