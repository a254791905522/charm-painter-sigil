# Publish Checklist - Charm Painter Sigil

## Identity
- [x] App name: Charm Painter Sigil
- [x] Name is 3 English words.
- [x] Bundle ID: com.rosewood.charmpaintersigil
- [x] Bundle ID contains `rosewood`.
- [x] PRODUCT_NAME: CharmPainterSigil
- [x] CFBundleDisplayName / CFBundleName: Charm Painter Sigil
- [x] Team ID configured: 7ZR52UNP43

## Source-Grounded Gameplay
- [x] Gameplay facts extracted from `SSCharmPainterScene.m`.
- [x] Metadata describes matching monster/spirit weakness to drawn rune.
- [x] Metadata mentions Flame, Frost, Rift, and Ward roles.
- [x] Metadata avoids generic rune-puzzle claims not supported by code.

## Template Residue / 4.3 Spam Risk
- [x] No `tw_*` resource names found.
- [x] No visible FPS/node debug overlay is enabled (`showsFPS = NO`, `showsNodeCount = NO`).
- [x] ReleaseProject resources synchronized with main project assets.
- [x] `image_prompts` is excluded from the Xcode target in `project.yml`.
- [x] App Store copy is written for this game, not copied from a previous title.

## iPhone Only
- [x] `TARGETED_DEVICE_FAMILY: '1'` in project-level settings.
- [x] `TARGETED_DEVICE_FAMILY: '1'` in target-level settings.
- [x] Final archive must show `UIDeviceFamily = (1)`.
- [x] Portrait orientation only is acceptable because the final app is iPhone-only.

## App Icon
- [x] `ASSETCATALOG_COMPILER_APPICON_NAME = AppIcon`.
- [x] `CFBundleIconName = AppIcon`.
- [x] Required icon PNG files exist: 120x120, 180x180, 152x152, 167x167, 1024x1024.
- [x] App icons are opaque with `hasAlpha: no`.
- [x] Re-check final archive for `Assets.car` and emitted `AppIcon*.png` after archive.

## Launch Screen
- [x] `UILaunchStoryboardName = LaunchScreen`.
- [x] `Base.lproj/LaunchScreen.storyboard` exists.
- [x] Re-check final archive for `Base.lproj/LaunchScreen.storyboardc`.

## App Store Metadata
- [x] `appstore-review-text.html` generated with textarea fields.
- [x] `keywords.txt` generated.
- [x] `README.md` generated.
- [x] `privacy.html` generated.
- [x] `index.html` generated with the LumiLink module structure.
- [x] Contact: xiao wangyu / +1 2096550297 / croitorzamkov@gmail.com

## Screenshots
- [x] 5 screenshots generated for 1284x2778.
- [x] 5 screenshots generated for 1242x2208.
- [x] Screenshots show menu, weakness reading, rune drawing, spirit wave, and result flow.

## Archive Verification
Run from `/Users/wxj/888ios/batch-game`:

```bash
xcodebuild \
  -project CharmPainter-ReleaseProject/CharmPainterSigil.xcodeproj \
  -scheme CharmPainter \
  -configuration Release \
  -sdk iphoneos \
  -archivePath /Users/wxj/888ios/batch-game/CharmPainter-Release/CharmPainterSigil.xcarchive \
  CODE_SIGNING_ALLOWED=NO \
  archive
```

Then inspect:

```bash
APP=/Users/wxj/888ios/batch-game/CharmPainter-Release/CharmPainterSigil.xcarchive/Products/Applications/CharmPainterSigil.app
/usr/libexec/PlistBuddy -c 'Print :CFBundleIdentifier' "$APP/Info.plist"
/usr/libexec/PlistBuddy -c 'Print :CFBundleDisplayName' "$APP/Info.plist"
/usr/libexec/PlistBuddy -c 'Print :UIDeviceFamily' "$APP/Info.plist"
find "$APP" -maxdepth 3 \( -name 'Assets.car' -o -name 'AppIcon*.png' -o -name 'LaunchScreen.storyboardc' \) -print | sort
```

## Deployment
- [x] Commit and push publish site to GitHub.
- [x] Deploy to Vercel with proxy `127.0.0.1:7897`.
- [x] Verify live URL: https://charm-painter-sigil.vercel.app
- [x] Verify privacy URL: https://charm-painter-sigil.vercel.app/privacy.html
