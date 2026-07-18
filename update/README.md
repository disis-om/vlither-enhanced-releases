# Signed Update Metadata

The active Android client will check these public endpoints:

```text
https://raw.githubusercontent.com/disis-om/vlither-enhanced-releases/main/update/latest.json
https://raw.githubusercontent.com/disis-om/vlither-enhanced-releases/main/update/latest.json.sig
```

`latest.json` and `latest.json.sig` are deliberately absent until the first
approved production release. This prevents an incomplete development build
from being advertised as an update.

The release publisher will generate both files atomically. They must never be
edited manually after publication.

The manifest contract will include, at minimum:

- schema version;
- product and package identity;
- version name and monotonically increasing version code;
- immutable GitHub Release APK URL;
- exact APK byte size and lowercase SHA-256 digest;
- publication time;
- headline, release notes, and OM Rajput creator credit.

The detached signature is verified by the public key bundled inside the
Android application before the APK is downloaded.
