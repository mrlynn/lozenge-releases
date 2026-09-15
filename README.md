# Lozenge for macOS

Signed and notarized downloads of **Lozenge**, the macOS teleprompter whose
window stays out of a full-desktop screen share.

This repository holds releases only. There is no source code here. The product
page is [lozenge.ai](https://lozenge.ai).

## Download

Open the [latest release](../../releases/latest) and download
`lozenge-<version>.dmg`. Open it and drag **Lozenge** to Applications.

Requires macOS 14 Sonoma or later, on Apple silicon or Intel.

## Check the download

Each release lists the SHA-256 of its DMG, and attaches it as
`lozenge-<version>.dmg.sha256`. In Terminal, in the folder you downloaded to:

```bash
shasum -a 256 lozenge-<version>.dmg
```

The line it prints must match the one in the release.

The app is signed with a Developer ID for Michael Lynn (team `YZ36Z8GSEN`) and
notarized by Apple. To see that for yourself after installing:

```bash
spctl --assess --type execute -v /Applications/Lozenge.app
```

It says `accepted` and `source=Notarized Developer ID`.

## Terms and privacy

Using Lozenge is covered by the [terms](https://lozenge.ai/terms) and the
[privacy policy](https://lozenge.ai/privacy).

## Questions

Write to [hello@lozenge.ai](mailto:hello@lozenge.ai).
