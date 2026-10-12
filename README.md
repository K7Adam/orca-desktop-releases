# Orca desktop builds (K7Adam fork)

Signed Windows installers of the private fork `K7Adam/orca` (branch `K7Adam/orca-wear`), built by
`.github/workflows/build-desktop-win.yml` whenever that branch moves. This repo holds binaries only.

- Installed fork builds update from this repo's releases; Orca's own "Update" keeps them on fork builds.
- Installers are signed with the fork's own certificate (`CN=K7Adam Orca Fork`). The updater installs a
  download only if it carries that signature, which needs the certificate in the user's trusted roots.
- `desktop/latest.json` records the last built source commit.
