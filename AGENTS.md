# CGI Timecards releases: instructions for coding agents (Codex and Claude)

## What this is
A PUBLIC repo that exists only so phones can download the CGI Timecards Android app and its update manifest from GitHub Releases. It holds no source code (just README.md and this file); the files phones use are release assets.

- Phones running 1.0.73 and newer read `version.json` from the latest release here. A pre-release named `dev-channel` carries test builds for the owner's phone.
- The permanent install link is https://github.com/stinjaco/cgi-timecards-releases/releases/latest/download/CGI_Timecards.apk
- Releases are made by `scripts/publish-release.ps1` in `cgi-timecards`, not by hand.

## Rules
- Everything here is world-readable. Never commit or upload keystores, signing passwords, tokens, API keys, `google-services.json`, employee names, hours or other company data.
- Never publish, edit, delete or re-upload a release (especially stable/latest) unless Jake explicitly says to; installed phones update from it. Follow the release steps in `cgi-timecards/AGENTS.md`.
- Extend, never rewrite: don't rename release assets or change the `version.json` shape.

## Related repos (all under github.com/stinjaco)
- `cgi-timecards` (private): the app's source and the release scripts; its `AGENTS.md` is the source of truth.
- `cgi-field-office`, `cgi-field-office-diagnostics`, `cgi-platform`: other CGI projects; nothing from them is published here.
