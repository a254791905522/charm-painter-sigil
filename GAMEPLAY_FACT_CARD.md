# Gameplay Fact Card - Charm Painter Sigil

## Source Evidence
- Core scene: `CharmPainterGame/SSCharmPainterScene.m`
- Menu scene: `CharmPainterGame/MainMenuScene.m`
- Level select: `CharmPainterGame/LevelSelectScene.m`
- Settings: `CharmPainterGame/SettingsScene.m`
- Bundle configuration: `CharmPainterGame/Info.plist`, `project.yml`

## Product Identity
- App name: Charm Painter Sigil
- Bundle ID: com.rosewood.charmpaintersigil
- Product name: CharmPainterSigil
- Platform: iPhone only
- Version: 1.0 (build 1)
- Team ID: 7ZR52UNP43

## Core Gameplay
Charm Painter Sigil is a portrait iPhone game where the player defeats descending spirits by drawing the correct charm rune. Each spirit shows a weakness label and HP. The player reads the front spirit, draws the matching symbol in the lower sigil box, and releases to cast. A matching rune damages the spirit; a wrong rune fizzles and gives no damage.

## Rune Rules
- Flame: recognized from a sideways zigzag stroke and used against Flame-weak spirits.
- Frost: recognized from a closed circle and used against Frost-weak spirits.
- Rift: recognized from a vertical zigzag stroke and used against Rift-weak spirits.
- Ward: recognized from a small closed loop and restores HP instead of attacking.

## Progression
- 50 local stages.
- Tutorial levels automatically hint/sync the target rune.
- Waves grow by level, with more spirits, faster descent, multiple lanes, and higher HP.
- Unlocked stage progress is stored locally with `CharmPainterUnlockedLevel`.

## Failure And Success
- Win condition: all spirits are cleared, then the game shows `SEAL RESTORED`.
- Lose condition: HP reaches zero or spirits cross the ward line, then the game shows `SEAL BROKEN`.
- Result overlay supports next level, restart, and menu actions.

## Visual Style
Dark Oriental Rune Fantasy: abyss black-purple background, indigo battle field, cyan/blue rune glow, dark stone panels, gold ritual accents, spirit enemies, and a lower drawing ward.

## Privacy / Monetization Facts
- Offline single-player.
- No account login.
- No ads.
- No in-app purchases.
- No analytics or tracking SDK detected in the project.
- Local settings store Music and Sound Effects toggles.
