# GitHub Update System

## Public request path

```text
Vlither Enhanced Android client
        -> signed update/latest.json
        -> detached signature verification
        -> version comparison
        -> user-approved backup
        -> GitHub Release APK download
        -> APK size, SHA-256, package, version, and certificate verification
        -> Android Package Installer
```

The update check runs asynchronously and must never block the title screen,
game input, or Play button.

## Sources shown by the client

The Check for Updates screen exposes two sources:

1. **GitHub Updates** - active.
2. **Official Publisher Updates** - reserved and disabled.

Only GitHub Updates participates in automatic checks. The disabled provider
must not issue background network requests.

## Release URL convention

```text
https://github.com/disis-om/vlither-enhanced-releases/releases/download/v1.1.0/Vlither-Enhanced-v1.1.0.apk
```

The APK is stored as a GitHub Release asset. It is not tracked as a normal Git
file.

## Client storage convention

Downloaded APKs are stored under:

```text
Download/Vlither Enhanced/
```

The Android client recreates its download folder when the user has deleted it.
Durable user backups use their own user-approved shared location and are not
bundled into APK downloads.

## Publication sequence

1. Complete and locally verify the application changes.
2. Build and verify an authorized production-signed APK.
3. Prepare the final changelog.
4. Create a draft GitHub Release and attach the APK.
5. Generate and sign the exact update manifest.
6. Verify the public APK bytes and signed metadata.
7. Publish only after explicit approval from OM Rajput.
