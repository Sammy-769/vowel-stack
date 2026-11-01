# Vowel Stack — Game Features and Functionality

## A. Game Overview

Vowel Stack is a portrait-oriented word puzzle with arcade survival and climbing mechanics. Letter tiles fall into a container while lava rises from below. Players select letters in an order that spells a valid word; submitting it clears those tiles and helps Cubey, the game's square companion, climb on word platforms or hold the lava back.

The project is suitable in concept for casual players who enjoy vocabulary puzzles and time pressure. This is an observation about the mechanics, not an age rating or a claim that the game teaches or tests English.

Its distinctive combination is the physical pile of falling, selectable letters, a rising hazard, and two different consequences for making words: building a route upwards in Levels or draining the lava in Endless.

## B. Gameplay and Game Modes

### Shared gameplay loop

1. Letter tiles spawn above the container at weighted random intervals and settle using 2D physics. The distribution favours common letters; the generator also tries to avoid repeating the two most recent letters.
2. The player clicks or taps tiles in the desired spelling order. Selected letters appear in a tray and are joined by a visual selection line. Tiles can be deselected.
3. A word is accepted when it is in the bundled word list and meets the mode's minimum length. Valid selections are submitted automatically after a short grace period (1.5 seconds by default); an invalid or too-short selection does not submit.
4. A valid word clears its selected tiles, awards points and XP, and then affects the mode objective. Tiles left behind continue to accumulate.

The usual minimum is three letters. Levels 9 and 10 require at least four letters. The word list is loaded locally, so basic word validation does not require an internet connection.

Letter values are broadly Scrabble-like (for example, vowels and common consonants are low value; J, Q, X and Z are high value). The score for a word is the sum of its letter values plus two points for every letter beyond the third. The current combo multiplier is then applied. A new valid word increments the combo; it expires after five seconds without another submitted word. Longer words have additional benefits that differ by mode.

### Modes

| Mode | Objective and progression |
|---|---|
| **Levels** | Ten configured levels with increasing/differing lava speeds, spawn intervals, tile limits and word-length requirements. Each valid word creates a labelled physical platform; Cubey automatically jumps onto platforms as they reach him. The objective is to climb to the goal marker before lava catches Cubey or letters overflow the container. A win unlocks the next level (up to the configured ten) and records score and challenge stars. |
| **Endless** | An open-ended survival mode with no goal marker. Valid words drain the lava according to their score; words of four or more letters give a larger drain multiplier. Cubey still climbs on word platforms, but the objective is to keep the rising lava and tile pile from reaching him for as long as possible. The run ends when Cubey is caught or the container overflows. Milestone combinations, scores, and word lengths can create additional bonus platforms. There is no final completion state in the implemented mode. |

In both modes, the run ends if Cubey touches the lava or the letter pile reaches its overflow conditions (a configured maximum tile count or the upper limit). Score is accumulated during the run and a personal best is kept separately for Endless and for each numbered level. A result screen offers replay/home navigation; successful level runs also offer the next level where one exists.

The configured Levels challenge set contains three star objectives per level:

| Level | Star objectives |
|---|---|
| 1 — First Steps | Win; make one 4-letter word; reach a ×2 combo |
| 2 — Getting Faster | Win; make a word worth 15+ points; reach a ×3 combo |
| 3 — Word Builder | Win; make two 4-letter words; score 80+ |
| 4 — Quick Thinking | Win; make a 5-letter word; reach a ×4 combo |
| 5 — Stay Cool | Win; score 110+; make a word worth 30+ points |
| 6 — Vocabulary Test | Win; use J, Q, X or Z in a word; reach a ×5 combo |
| 7 — No Easy Escape | Win and reach ×4; make three words of 4+ letters; win without using a power-up |
| 8 — Long Word Master | Win and make a 30+ point word; make a 6-letter word; reach a ×6 combo |
| 9 — Under Pressure | Win and make a 4+ letter word; make two 5+ letter words; score 160+ |
| 10 — Cubey’s Final Escape | Win and make a 4+ letter word; make two 6+ letter words; reach a ×4 combo |

Stars are recorded on a level victory, retained as the best collected for that level, and can be earned across repeat attempts. A level has a configured maximum coin budget for all three stars; rewards are paid proportionally as new stars are earned.

## C. Power-ups and Special Mechanics

The local profile starts with two charges of each power-up. A charge is consumed on activation; if none remain, the in-game button can purchase and immediately use one if the player has enough coins. The Store separately sells additional inventory.

| Power-up | Effect | Conditions and cost when used without a stored charge |
|---|---|---|
| **Slow Motion** | Sets game time scale to 50% for six seconds, making tile selection easier. The duration is measured independently of the slowed game clock. | One active use at a time; 170 coins for a direct purchase. |
| **Freeze Lava** | Stops the lava hazard for six seconds, with a visual ice effect. | One active use at a time; 200 coins for a direct purchase. |
| **Platform Drop** | Drops an empty safety platform from above for Cubey to climb. | Available during Levels, not usable during Endless; 150 coins for a direct purchase. |

During active play, a rare falling box can occasionally appear after two minutes of gameplay. It contains one randomly selected Slow Motion, Freeze or Platform Drop charge. Collecting it requires ten rapid taps within 3.2 seconds; the box also falls through the scene and is missed if it reaches the bottom first. Platform Drop charges collected in Endless are saved for later Levels.

Other special mechanics include a valid-word grace timer, combo feedback, an emergency hint from Cubey after inactivity when a common word can be formed, and a “clutch” lava retreat for certain meaningful words made close to the hazard. These provide feedback or relief; they do not replace the core word rules.

## D. Progression and Daily Challenges

### Level and score progression

- The first numbered level is initially unlocked. Winning a level advances the saved unlock value and makes the next configured level available.
- Each level tracks up to three challenge stars, the best score, and cumulative completed-level state.
- The game awards coins after a run equal to half of its score (integer division); a Level victory can add the level’s newly earned star reward.
- High scores are saved per mode/level. The overall leaderboard score is the sum of the Endless personal best and each numbered-level personal best.

### Daily Word

The game chooses one target word per system-calendar date from a small built-in set of familiar three-, four- and five-letter words. The selection is deterministic for the date, so reopening the game does not reroll that day’s target. Making that exact word in either game mode marks the challenge complete; the reward must then be claimed from its lobby panel.

| Target length | Claim reward |
|---|---:|
| 3 letters | 100 coins |
| 4 letters | 200 coins |
| 5 letters | 300 coins |

The date, target, viewed/completed/claimed state are saved. Daily Word completion is checked when a valid word is submitted. The in-game prompt says to make the word in Levels or Endless. Because Levels 9–10 reject words shorter than four letters, a three-letter daily target must be completed in Endless or an earlier level.

### Seven-day Daily Rewards

The lobby offers a separate seven-claim reward track. One reward can be claimed per calendar date; missing a day does not reset progress. The sequence is:

1. 200 coins
2. 400 coins
3. Rose Pink Cubey colour
4. Alpine Trail background
5. Cat Ears outfit
6. DynaPuff font
7. 1,000 coins

Availability uses the device’s system date. Daily features are local-gameplay features and do not require a live challenge server; signed-in profiles include their claim state in cloud profile metadata.

## E. Cubey Character System

Cubey is both the climbing character and a contextual dialogue companion. In gameplay he jumps automatically onto reachable word platforms. In the lobby he reacts to taps, double taps, repeated taps, swipes and long presses, and provides occasional idle dialogue. In a run he can react to words, combos, rare letters, danger, successful escapes, invalid selections and inactivity.

### XP and dialogue ranks

Every submitted word awards XP equal to the points scored for that word, including its combo multiplier. Cumulative XP unlocks the following display ranks:

| Rank | XP threshold |
|---|---:|
| A1 | 0 |
| A2 | 1,000 |
| B1 | 3,000 |
| B2 | 6,000 |
| C1 | 10,000 |
| C2 | 15,000 |

The rank unlocks additional lines of Cubey dialogue. The lobby’s progress panel displays the current rank, XP progress and unlocked sentences in Lobby, Idle, Jump, Combo, Danger and Escape categories. Reaching a new rank triggers a celebration and the interface describes it as Cubey learning new sentences.

These are game progression labels and scripted dialogue unlocks, not an assessment of the player. The game does not evaluate English proficiency, grammar, reading ability or educational attainment. Its word acceptance is based on dictionary membership and game rules.

Cubey also keeps bounded local memory such as recent/favourite words, longest word, combos, run outcomes, invalid attempts, power-up use and lobby interactions. This supports reactive dialogue. This memory is not included in the Cloud upload payload inspected.

## F. Customisation

The Store allows cosmetic inventory to be purchased with in-game coins and equipped. The default colour, no outfit, default font and first background are available without purchase. Some items are also granted through the daily reward track.

| Customisation | Available options |
|---|---|
| **Cubey colours** | Meadow Green (default), Sky Blue, Coral Red, Golden Yellow, Rose Pink and Cocoa Brown. Each non-default colour is 300 coins. |
| **Outfits** | None (default), Top Hat (300), Wizard Hat (400), Cat Ears (300), Royal Crown (700), Graduation Cap (600), Chef Hat (450), Pirate Hat (500) and Party Hat (400). Prices are coins. |
| **Letter font** | Default Font, Rainbow2000 (350), DynaPuff (500), Fredoka (300), Free Cheese (450), Gluten (550), Rubik Bubbles (700), Scabber (650), Sniglet (600) and TypeLight Sans (400). Prices are coins. The selected font is applied to letter tiles. |
| **Background** | Meadow Falls (free/default), Golden Dusk (500), Alpine Trail (700), Crystal River (800) and Moonlit Valley (900). Prices are coins. |

Cosmetic previews appear in the Store. Equipped colour and outfit alter Cubey’s appearance; selected backgrounds are applied in gameplay and the game lobby.

## G. Leaderboard and Online Features

The project integrates the bundled **SilentWolf 0.9.9** Godot plugin. The game uses SilentWolf’s scores service as a profile/leaderboard store:

- The leaderboard requests the `player_accounts` board, removes duplicate profile rows and presents a podium/list, local-player rank and profile cards.
- The displayed profile includes the player name, combined best score, coin total, XP/rank, profile message, equipped cosmetics and selected owned items.
- Players can edit a profile message (up to 150 characters); local filtering is applied before saving and again when displayed.
- The game tracks top-ten rank notifications and presence/last-seen information in profile metadata.
- A separate `game_config` leaderboard is queried for remote update announcements, with an HTTPS download link opened externally when available.

The account screen implements local username/password checks and registration/login requests through the project’s Cloud script and SilentWolf score metadata. The plugin also contains account/authentication interfaces, but this project path should not be assumed equivalent to an independently verified production authentication service.

SilentWolf multiplayer code is bundled, but the game’s Multiplayer menu displays “Coming Soon”; no active multiplayer match flow was found. The bundled plugin contains WebSocket multiplayer modules, but the game does not appear to invoke them.

Online account sync, leaderboard, rank lookup, update announcements and external sponsored-link rewards need network access and a working SilentWolf service configuration. The project includes configured SilentWolf API settings in plugin source; no credential values are reproduced here. A buyer should obtain buyer-controlled service configuration and have any embedded key securely reviewed/replaced. The seller’s accounts, service entitlements or cloud records are not represented as transferable.

## H. Saving and Data Management

### Local save

The Save singleton stores the local profile under Godot’s `user://` data location using Godot’s encrypted file API. Saved fields include username/login state, coins, unlocks, completed levels, scores, XP, stars, inventories and equipped cosmetics, daily reward/word state, and profile/rank notification state. Schema migrations add or normalise fields for newer versions.

Music volume, Cubey’s bounded memory and the Store sponsored-reward cooldown are local state. The embedded save encryption key is part of the project source; this should not be treated as strong protection against a person with access to the project or device.

### Cloud save and offline play

The project saves locally first. In guest/offline mode it skips Cloud uploads, so the main word gameplay, local progression, daily features and Store continue without sign-in or an active connection. A network connection is required to register or log in, sync a signed-in profile, load the online leaderboard/rank, check remote update notices, or complete the sponsored-link flow.

On sign-in, Cloud attempts to merge local and online progress. The sync payload contains profile identity/device metadata and gameplay progress such as coins, scores, level unlocks, XP, stars, power-up inventories, customisation and daily states. Personal bests and XP are merged using maximum values; other profile data is resolved using save revision and timestamp logic. A failed sync does not remove the local-first save, but online features may show unavailable/error states until a service request succeeds.

The project’s account code calculates a `String.hash()` integer for the password and includes that value in cloud score metadata. It is not evidence of a hardened authentication design; a buyer should review account security and migration requirements before production use. Do not rely on the local save encryption or current account flow as a security boundary without a separate review.

## I. User Interface and Menus

| Screen or panel | Purpose |
|---|---|
| **Title lobby** | Play navigation, guest/offline choice, account registration and login, Store, Support, exit and Multiplayer placeholder. |
| **Game lobby** | Levels and Endless selection; coin/high-score/profile summary; XP/rank widget; Daily Rewards, Daily Word and online leaderboard panels; Cubey interactions; Discord link. |
| **Level selection** | Ten level cards with lock state, saved stars and best score. |
| **Gameplay HUD** | Score, coins, selectable tile tray, pause control and power-up controls. Level mode also shows goal and level challenge progress. |
| **Pause panel** | Resume, return to lobby, current Level challenge progress and music-volume slider. |
| **Victory / Try Again panels** | Run score and coin result, earned challenge stars on Levels, home/replay/next-level options, and a sponsored-link reward option. |
| **Store** | Rewards, power-ups, outfits/colours, fonts and backgrounds. |
| **Support** | Developer support information and copyable cryptocurrency donation destinations. |
| **Leaderboard/profile overlays** | Online ranking and player profile details. |
| **Update notice** | Dismissible remote release announcement with optional external HTTPS download link. |

The code includes mobile back-button handling, touch gestures for relevant tabs/panels, and mouse-to-touch emulation. No separate in-game tutorial, comprehensive help screen, or implemented achievements collection was identified.

## J. Audio and Visual Experience

The presentation uses bright pastel letter tiles and platforms, a stylised square companion, colourful backgrounds and rounded, animated interface panels. Valid-word clears use staged tile pops, score feedback, particles, combo effects and camera shake. Lava receives a near-danger treatment and a blue ice shader while frozen. Background parallax can use gravity/accelerometer and gyroscope input on devices that provide those sensors.

The project includes separate lobby music, gameplay music and sound effects for tile selection/collisions, word results, combos, power-ups, rewards, notifications, jumps and victories. A music-volume slider is available in the gameplay pause panel and the value is saved locally. No separate SFX volume control was found.

## K. Technical Overview

- **Engine:** Godot project format version 5; `project.godot` declares Godot feature version **4.7** and GL Compatibility rendering.
- **Display/input configuration:** 720 × 1280 portrait-oriented viewport, canvas-item stretch, accelerometer/gravity/gyroscope enabled, and touch-to-mouse emulation enabled.
- **Export presets:** Web and Android presets are present in `export_presets.cfg`. Their presence is not evidence that a release build was tested or that store signing/release accounts are included.
- **Core systems:** GDScript singletons for Save, Cloud, Global rules, word lookup, audio, effects, ads and update notices; scene-based Levels, Endless, Store, lobby and gameplay; 2D physics for tiles/platforms and the rising lava hazard.
- **Third-party integration:** SilentWolf plugin 0.9.9; Godot/Jolt physics integration. No separate game SDK/library beyond those integrations was identified in the project source inspected.
- **External endpoints:** SilentWolf scores/cloud service; Effective CPM Network smartlink; Google connectivity-check endpoint; Discord invite. External accounts and service terms are outside the Godot project.

## L. Current Implementation and Limitations

### Implemented in project code

- Local Levels and Endless gameplay, physics-based letter spawning, dictionary validation, word scoring, combos, rising-lava and overflow outcomes.
- Ten configured Levels, challenge-star tracking, progression, coin economy, power-ups and cosmetic Store.
- Daily Word and seven-claim Daily Rewards.
- Cubey’s rank-based dialogue, contextual reactions and local bounded memory.
- Local save/load and a SilentWolf-backed account/profile, Cloud sync and leaderboard integration.
- Music/audio feedback, gameplay result/pause panels, online update notice and external sponsored-link reward flow.

### Partial, externally dependent or requiring testing

- SilentWolf authentication, profile sync, leaderboard, remote updates and rank/presence require the configured service and network. Their current availability, account ownership, service terms and buyer transferability are not established by source inspection.
- Sponsored-link “rewarded ad” buttons open an external SmartLink, then infer completion from the app losing focus for at least three seconds and returning with connectivity. The project does not show a verified ad-network impression/completion callback. Whether the network offers suitable content or pays out requires external confirmation.
- The one-time revive is offered only after a lava-contact loss, only if connectivity is available, and at most once per run. It is not available for overflow losses. It uses the same sponsored-link return flow.
- Multiplayer is explicitly presented as coming soon; functional multiplayer is not implemented in the game flow.
- Web and Android export configurations exist, but no build, store deployment, signing setup or device compatibility test is claimed here.
- No gameplay runtime test was performed for this document. The descriptions reflect source and scene inspection, not a guarantee of defect-free behaviour.

### Other limitations and items for buyer review

- Dictionary provenance/licensing and several asset rights remain unverified; see the project’s asset-credit and licence-verification documents.
- The word list must be present in the project for validation; if it cannot load, the dictionary manager reports an error and valid-word submission cannot operate normally.
- Daily schedules rely on the device’s system date.
- The account implementation’s password-hash handling and embedded service configuration merit security/ownership review before a public release. No credential values are included in this document.
- The project includes donation copy and cryptocurrency-address copy buttons in the Support screen; confirm ownership and whether those should be removed or replaced for the buyer.
- No formal language assessment, lesson curriculum, multiplayer matchmaking, achievements system or verified advertising SDK is present in the implemented flow.

## M. Project Handover

The Godot project folder contains:

- **GDScript source:** gameplay, UI, save/progression, word validation, audio/effects, Cloud, SilentWolf calls, Store, update and external-link logic.
- **Scenes and resources:** title/game lobbies, Levels and Endless entry, gameplay, Store, Support, leaderboard/profile panels, UI overlays and reusable Cubey, letter, lava and platform scenes.
- **Assets:** audio, fonts, backgrounds, interface graphics, character/outfit art, the word list and Cubey dialogue text.
- **Configuration:** `project.godot`, import metadata, Web/Android export presets and Android build/export material present in the folder.
- **Third-party code:** the bundled SilentWolf plugin and its assets. Plugin rights and service arrangements require separate confirmation.
- **Existing buyer documentation:** asset credits, third-party dependencies and licence-verification checklists are present in the project root.

The project folder does not itself transfer third-party licences, external service subscriptions, seller-owned SilentWolf or advertising accounts, leaderboard/cloud data, Discord community ownership, platform developer accounts, signing credentials or ad-network entitlements. These must be independently reviewed and arranged between the parties.
