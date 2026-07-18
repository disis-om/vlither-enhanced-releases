# Release Policy

## One public update stream

Vlither Enhanced uses one normal public update stream. Public releases use
semantic versions such as `1.1.0`, `1.1.1`, and `1.2.0`. This repository does
not expose separate alpha, beta, development, or stable channels to the app.

## Approval boundary

Creating repository files does not authorize an APK release. A release may be
published only after OM Rajput explicitly approves the exact version,
production-signed APK, and final changelog.

## Required gates

Before publication, the release workflow must verify:

1. Application ID `com.vlither.enhanced`.
2. A version code higher than every previously published build.
3. The expected production signing-certificate fingerprint.
4. The exact APK byte size and SHA-256 digest.
5. A valid detached signature for the exact update-manifest bytes.
6. HTTPS download URLs hosted by the approved GitHub repository.
7. Creator credit to OM Rajput and a precise, factual changelog.

## Immutability

A published tag, APK asset, manifest snapshot, or changelog must not be
silently replaced. If a defect is discovered, publish a newer version with a
higher version code.

## Forbidden content

The repository must never contain private application source, signing
keystores, signing passwords, manifest private keys, GitHub tokens, Termux
secrets, or deployment credentials.
