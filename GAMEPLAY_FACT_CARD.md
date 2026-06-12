# Gameplay Fact Card - Charm Painter Sigil

- Game type: portrait iPhone rune drawing puzzle / light arcade defense.
- Theme: dark oriental rune fantasy, abyss-purple ritual field, glowing sigils, spirit enemies, ancient seal restoration.
- Core loop: read the front spirit weakness, draw the matching rune in the bottom sigil box, release to cast, clear the wave before spirits cross the ward.
- Rune set: Flame, Frost, Rift, Ward.
- Recognition rules: closed loops, zigzag-like strokes, and small ward loops are recognized from player stroke points.
- Progression: 50 local stages, unlocked with `CharmPainterUnlockedLevel` in `NSUserDefaults`.
- Difficulty: spirits increase from 2 up to 12 per stage, HP increases over time, later waves add faster lane pressure and bonus HP spirits.
- Fail state: spirits reaching the draw ward reduce HP; if HP reaches zero the seal breaks.
- Win state: removing all spirits restores the seal and unlocks the next level.
- Controls: Continue, Stages, Settings, result Next Level, Restart, Menu.
- Settings: Music and Sound Effects toggles stored locally.
- Privacy: offline single-player; no login, ads, purchases, analytics, or network gameplay dependency found in source.
- Release identity: Bundle ID `com.rosewood.charmpaintersigil`, display name `Charm Painter Sigil`, iPhone only.
