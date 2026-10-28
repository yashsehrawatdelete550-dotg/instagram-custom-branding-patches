# Instagram Custom Branding patches for Morphe

This repository contains a **patch component**, not yet a built Morphe patch bundle. It cannot be added to Morphe Manager as a working source until it is integrated into the official Morphe Patches Template and a compatible `.mpp` bundle is built and tested.

## Included patch options
- Custom app name: Instagram PRO 👑, InstagramPRO👑, or a custom label.
- Custom app icon: replace launcher/alternate icon resources from a PNG path.
- Custom splash text: keep, replace, or hide the “from Meta” text and choose its color.

## Build status
**Not verified yet.** This code has not been compiled against the current Morphe template or tested on an Instagram APK. The icon replacement logic also needs validation against the target Instagram resource layouts before use.

## Next steps
1. Integrate the `patches/` directory into a compatible fork of the official template: https://github.com/MorpheApp/morphe-patches-template
2. Include the required `patches/src/main/resources/branding/font_33.bin` and `font_44.bin` resources from the original project for the splash-text renderer.
3. Run the template's build/release workflow and inspect the build logs.
4. Test the generated `.mpp` bundle with Morphe Manager and a supported Instagram APK.
5. Only after a successful build and test, add this repository as a remote source in Morphe.

## Add source in Morphe
Morphe accepts GitHub repository sources, but a repository must expose a compatible bundle/release; merely uploading Kotlin source files is not enough. See the official guide: https://github.com/MorpheApp/morphe-manager/blob/main/docs/patch-sources.md

Do not use this repository to patch an app until the build and runtime behavior have been verified.
