# TOTEMSurf update mirror

Public mirror of TOTEMSurf's signed update policy:

- `update-policy.json` — newest and minimum supported version per platform
- `update-policy.json.sig` — Ed25519 signature over the exact bytes of that file

TOTEMSurf reads these from here when it cannot reach `update.totemsurf.app`,
and accepts them only if the signature verifies against the key built into the
app. Nothing in this repository can change what the app does unless it was
signed with the release key; editing these files here only makes the app
ignore them.

Installers: see the Releases of this repository, or
https://totemapps.com/totemsurf/download/

Maintained by `tools/publish_update_mirrors.sh` in the TOTEMSurf source tree.
