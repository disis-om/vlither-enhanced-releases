# Vlither Enhanced Releases

Official Android release distribution for **Vlither Enhanced**, developed and
maintained by **OM Rajput**.

This repository is intentionally limited to public release metadata,
changelogs, and verified APK assets. The private application source, signing
material, deployment credentials, and update-signing keys are not stored here.

## Current status

Vlither Enhanced `1.1.0` is in active development. No public APK has been
released from this repository yet.

When the first approved release is ready, it will appear in the repository's
[Releases](../../releases) section. The Android client will obtain update
metadata from the signed files under `update/`.

## Update model

- **GitHub Updates** is the active update source.
- **Official Publisher Updates** is reserved for future use and remains
  disabled in the client.
- Every published APK must have a monotonically increasing Android version
  code.
- Every APK must match the package identity and production signing certificate
  expected by the installed application.
- Update metadata must be signed and must contain the exact APK size and
  SHA-256 digest.
- Published versions are immutable. A correction is delivered as a newer
  version instead of replacing historical bytes.

## Public files

```text
update/       Signed latest-release metadata
changelogs/   User-facing release notes
docs/         Public update-system documentation
```

APK binaries are attached to GitHub Releases; they are not committed to the
Git repository.

## Product identity

**Vlither Enhanced**

The Arena, Re-Engineered.

Developed and maintained by **OM Rajput**.
