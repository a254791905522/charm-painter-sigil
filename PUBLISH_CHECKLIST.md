# Charm Painter Sigil Publish Checklist

## Gameplay Facts

- The player draws rune shapes to cast charms against descending spirits.
- Each spirit shows a weakness label and HP.
- Correct rune casts damage; wrong rune casts fizzle; Ward restores HP.
- The game has 50 local stages and stores unlock progress on device.
- Visual theme: dark oriental rune fantasy with abyss-purple backgrounds, cyan/gold sigil glow, stone buttons, and spirit enemies.

## Release Identity

- App name: Charm Painter Sigil
- PRODUCT_NAME: CharmPainterSigil
- CFBundleDisplayName: Charm Painter Sigil
- CFBundleName: Charm Painter Sigil
- Bundle ID: com.rosewood.charmpaintersigil
- Team ID: 7ZR52UNP43
- Version: 1.0
- Build: 1
- Device support: iPhone only
- iPad support: No

## Files Generated

- `GAMEPLAY_FACT_CARD.md`
- `PUBLISH_CHECKLIST.md`
- `appstore-review-text.html`
- `keywords.txt`
- `README.md`
- `index.html`
- `privacy.html`
- `screenshots-1284x2778/*.png`
- `screenshots-1242x2208/*.png`

## App Store Metadata

- Subtitle: Draw Runes, Seal Spirits
- Promotional text: Read each spirit weakness, draw glowing runes, restore the seal, and clear 50 offline sigil stages.
- Keywords: rune,sigil,charm,puzzle,drawing,magic,offline,levels,spirits,seal
- Category: Games / Puzzle
- Age rating recommendation: 4+
- Support URL: https://charm-painter-sigil.vercel.app
- Marketing URL: https://charm-painter-sigil.vercel.app
- Privacy URL: https://charm-painter-sigil.vercel.app/privacy.html

## Preflight Checks

- [ ] `project.yml` and `.xcodeproj` agree on Bundle ID and iPhone-only settings.
- [ ] `CFBundleIconName = AppIcon`.
- [ ] App icons include 120x120, 180x180, and 1024x1024 with no alpha.
- [ ] `UILaunchStoryboardName = LaunchScreen`.
- [ ] Final archive contains `Base.lproj/LaunchScreen.storyboardc`.
- [ ] Final archive `UIDeviceFamily` contains only `1`.
- [ ] Final archive contains `Assets.car` and emitted AppIcon PNGs.
- [ ] No `tw_*` resources remain.
- [ ] No visible FPS/node debug overlay is enabled.
- [ ] App Store text is specific to rune drawing, spirit weaknesses, and seal restoration.

## Contact

- Name: xiao wangyu
- Phone: +1 2096550297
- Email: croitorzamkov@gmail.com
