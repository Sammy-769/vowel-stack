# Vowel Stack — Asset Credits and Inventory

## Scope and counting method

This inventory covers the unique source assets in the project: **86 files** — 17 audio files, 10 fonts, 57 images/graphics, and 2 language/text resources. SilentWolf's bundled media is included in the font and image counts; the plugin itself is covered in [THIRD_PARTY_DEPENDENCIES.md](./THIRD_PARTY_DEPENDENCIES.md).

Godot import sidecars (`*.import`), the generated `.godot/` cache, and build outputs under `android/build/` are not counted as separate assets. Licence/README files are documentation accompanying assets, not game assets.

## Audio — 17 files

All sound effects were sourced from Pixabay and both music tracks from StockTune. I checked the relevant platform licences when selecting these assets and chose them for use in the game, including commercial use.

### Pixabay sound effects

The Pixabay Content License permits commercial use of sound effects, subject to its terms and restrictions. The full terms are at the [Pixabay Content License Summary](https://pixabay.com/service/license-summary/) and [full terms](https://pixabay.com/service/terms/).

| Game sound | Current project filename and location | Asset | Source page |
|---|---|---|---|
| Victory | `assets/audio/game/victory.mp3` | Level Up 08 | [Pixabay](https://pixabay.com/sound-effects/film-special-effects-level-up-08-402152/) |
| Freeze | `assets/audio/game/freeze.mp3` | Iced Magic 6 | [Pixabay](https://pixabay.com/sound-effects/film-special-effects-iced-magic-6-378606/) |
| Notification | `assets/audio/game/notification.mp3` | New Notification 051 | [Pixabay](https://pixabay.com/sound-effects/technology-new-notification-051-494246/) |
| Slow motion | `assets/audio/game/slow_motion.mp3` | Slowdown FX | [Pixabay](https://pixabay.com/sound-effects/film-special-effects-slowdown-fx-343685/) |
| Money | `assets/audio/money/money.mp3` | Cashier "Ka-ching" Sound Effect | [Pixabay](https://pixabay.com/sound-effects/film-special-effects-cashier-quotka-chingquot-sound-effect-129698/) |
| Error | `assets/audio/money/error.mp3` | UI Error Pop | [Pixabay](https://pixabay.com/sound-effects/film-special-effects-ui-error-pop-515668/) |
| Pop | `assets/audio/pop/pop.mp3` | Pop | [Pixabay](https://pixabay.com/sound-effects/film-special-effects-pop-402324/) |
| Balloon pop | `assets/audio/pop/balloon pop.mp3` | Balloon Pop Sound Effect | [Pixabay](https://pixabay.com/sound-effects/film-special-effects-balloon-pop-sound-effect-504628/) |
| Pop select | `assets/audio/pop/pop_select.mp3` | Multi Pop 2 | [Pixabay](https://pixabay.com/sound-effects/film-special-effects-multi-pop-2-188167/) |
| Platform | `assets/audio/platform/platform.mp3` | Body Fall | [Pixabay](https://pixabay.com/sound-effects/film-special-effects-body-fall-142378/) |
| Platform 3 | `assets/audio/platform/platform3.mp3` | Heavy Body Fall | [Pixabay](https://pixabay.com/sound-effects/film-special-effects-heavy-body-fall-352446/) |
| Platform 2 | `assets/audio/platform/platform2.mp3` | Character Fall Impact | [Pixabay](https://pixabay.com/sound-effects/film-special-effects-character-fall-impact-352287/) |
| Reward | `assets/audio/game/reward.mp3` | Achievement Badge Pop Sound 1 | [Pixabay](https://pixabay.com/sound-effects/film-special-effects-achievement-badge-pop-sound-1-547860/) |

Two further sound effects were also downloaded from Pixabay, but I no longer have the individual asset-page links for them:

| Current project filename and location | Source |
|---|---|
| `assets/audio/game/combo.mp3` | Pixabay |
| `assets/audio/money/coin.mp3` | Pixabay |

### StockTune music

Both music tracks were sourced from StockTune. StockTune's [Use License and Terms](https://stocktune.com/info/terms) state that its content is public domain and may be used, shared and adapted for personal and commercial purposes. The terms also ask users to act responsibly and ethically, prohibit implying endorsement without permission, and note that StockTune may not own or have created all supplied content.

| Game music | Current project filename and location | Track | Source page |
|---|---|---|---|
| In-game music | `assets/audio/music/game_music.ogg` | Echoes of Childhood Dreams | [StockTune](https://stocktune.com/free-music/echoes-of-childhood-dreams-230054-140085) |
| Lobby music | `assets/audio/music/lobby_music.ogg` | Memories in Slow Motion | [StockTune](https://stocktune.com/free-music/memories-in-slow-motion-230053-140085) |

## Fonts — 10 files

Five font folders contain SIL Open Font License 1.1 notices naming the project authors. Four font folders contain CC0 1.0 legal text. Comfortaa is bundled with the SilentWolf addon. SilentWolf's official [FAQ](https://silentwolf.com/) answers "Can I use SilentWolf in a commercial game?" with "Yes! You can use SilentWolf in games that make money." — which confirms commercial use of the bundled font as part of the addon.

| Current project filename and location | Source and licence information |
|---|---|
| `assets/fonts/DynaPuff/DynaPuff-VariableFont_wdth,wght.ttf` | SIL OFL 1.1. `OFL.txt` names The DynaPuff Project Authors. Source: https://github.com/googlefonts/dynapuff |
| `assets/fonts/Fredoka/Fredoka-Medium.ttf` | SIL OFL 1.1. `OFL.txt` names The Fredoka Project Authors. Source: https://github.com/hafontia/Fredoka-One |
| `assets/fonts/FreeCheese_Font_1_0/FreeCheese-Regular.ttf` | Folder contains CC0 1.0 legal text (`License.txt`). |
| `assets/fonts/Gluten/Gluten-Medium.ttf` | SIL OFL 1.1. `OFL.txt` names The Gluten Project Authors. Source: https://github.com/Etcetera-Type-Co/Gluten |
| `assets/fonts/Rainbow2000_Font_v1_04/Rainbow2000-Bold.ttf` | Folder contains CC0 1.0 legal text (`License.txt`). |
| `assets/fonts/Rubik_Bubbles/RubikBubbles-Regular.ttf` | SIL OFL 1.1. `OFL.txt` names The Rubik Filtered Project Authors. The notice's source URL is malformed; the intended project is Rubik-Filtered on GitHub. |
| `assets/fonts/scabber-font/Scabber-q2Mn0.ttf` | Folder contains CC0 1.0 legal text (`License-473a.txt`). |
| `assets/fonts/Sniglet/Sniglet-ExtraBold.ttf` | SIL OFL 1.1. `OFL.txt` names Haley Fiege, Brenda Gallo and Pablo Impallari. |
| `assets/fonts/type-light-sans-font/TypeLightSans-KV84p.otf` | Folder contains CC0 1.0 legal text (`License-473a.txt`). |
| `addons/silent_wolf/assets/fonts/Comfortaa-Bold.ttf` | Bundled with SilentWolf. SilentWolf's official [FAQ](https://silentwolf.com/) confirms commercial-game use of the addon. |

## Images and graphics — 57 files

Most of the game's graphics were generated using OpenAI's ChatGPT image-generation capabilities. Under OpenAI's [Terms of Use](https://openai.com/policies/row-terms-of-use/), OpenAI assigns to the user its rights in generated output to the extent permitted by law. The individual generation histories for these images are not retained, so the tables below record the general source rather than a per-file record.

### Backgrounds and mode graphics — 11 files

All generated with ChatGPT. See OpenAI Terms of Use above.

| Current project filename and location |
|---|
| `assets/sprite/background/bg1.png` |
| `assets/sprite/background/bg2.png` |
| `assets/sprite/background/bg3.png` |
| `assets/sprite/background/bg4.png` |
| `assets/sprite/background/bg5.png` |
| `assets/sprite/background/endless icon.png` |
| `assets/sprite/background/endless_tumb.png` |
| `assets/sprite/background/levels icon.png` |
| `assets/sprite/background/levels.png` |
| `assets/sprite/background/levels_tumb.png` |
| `assets/sprite/background/lobby.png` |

### Interface buttons — 16 files

All generated with ChatGPT. See OpenAI Terms of Use above.

| Current project filename and location |
|---|
| `assets/sprite/buttons/achievements.png` |
| `assets/sprite/buttons/ad button.png` |
| `assets/sprite/buttons/back button.png` |
| `assets/sprite/buttons/daily word.png` |
| `assets/sprite/buttons/discord.png` |
| `assets/sprite/buttons/freeze.png` |
| `assets/sprite/buttons/gift.png` |
| `assets/sprite/buttons/home green.png` |
| `assets/sprite/buttons/home red.png` |
| `assets/sprite/buttons/leaderboard.png` |
| `assets/sprite/buttons/nextlevel.png` |
| `assets/sprite/buttons/pause button.png` |
| `assets/sprite/buttons/platform drop.png` |
| `assets/sprite/buttons/progress.png` |
| `assets/sprite/buttons/slowmo.png` |
| `assets/sprite/buttons/tryagain button.png` |

### Gameplay objects and character parts — 9 files

All generated with ChatGPT. See OpenAI Terms of Use above.

| Current project filename and location |
|---|
| `assets/sprite/game sprite/coin.png` |
| `assets/sprite/game sprite/display podium.png` |
| `assets/sprite/game sprite/frame.png` |
| `assets/sprite/game sprite/land.png` |
| `assets/sprite/game sprite/lava.png` |
| `assets/sprite/game sprite/rock.png` |
| `assets/sprite/game sprite/star.png` |
| `assets/sprite/player/eyes.png` |
| `assets/sprite/player/mouth.png` |

### Cubey outfits — 8 files

All generated with ChatGPT. See OpenAI Terms of Use above.

| Current project filename and location |
|---|
| `assets/sprite/outfits/birthday.png` |
| `assets/sprite/outfits/cat ears.png` |
| `assets/sprite/outfits/chef.png` |
| `assets/sprite/outfits/crown.png` |
| `assets/sprite/outfits/graduation cap.png` |
| `assets/sprite/outfits/pirate.png` |
| `assets/sprite/outfits/top hat.png` |
| `assets/sprite/outfits/wizard.png` |

### UI and project branding — 6 files

All generated with ChatGPT. See OpenAI Terms of Use above.

| Current project filename and location |
|---|
| `assets/sprite/ui/adaptive_icon_background.svg` |
| `assets/sprite/ui/adaptive_icon_foreground.png` |
| `assets/sprite/ui/tryagain.png` |
| `assets/sprite/ui/victory.png` |
| `boot image.png` |
| `gameicon.png` |

### Crypto-address graphics — 2 files (to be removed before handover)

These are screenshots, not AI-generated artwork. I plan to delete both after the sale is confirmed and before handing over the project.

| Current project filename and location |
|---|
| `assets/sprite/crypto address/ton.png` |
| `assets/sprite/crypto address/usdt(TRC20).png` |

### Bundled SilentWolf plugin graphics — 5 files

These graphics are bundled with the SilentWolf addon. SilentWolf's official [FAQ](https://silentwolf.com/) confirms that SilentWolf may be used in games that make money, which covers use of its bundled graphics as part of the addon in a commercial game. The FAQ is not a separate standalone licence for extracting or reselling individual plugin assets.

| Current project filename and location |
|---|
| `addons/silent_wolf/assets/gfx/checkbox_checked.png` |
| `addons/silent_wolf/assets/gfx/checkbox_unchecked.png` |
| `addons/silent_wolf/assets/gfx/dummy_info_icon_small.png` |
| `addons/silent_wolf/assets/gfx/info_icon.png` |
| `addons/silent_wolf/assets/gfx/info_icon_small.png` |

## Language and dialogue resources — 2 files

| Current project filename and location | Purpose and source/licence |
|---|---|
| `assets/data/words_list.txt` | 370,105 entries used by the local word manager for dictionary validation. The associated licence text is in [`assets/data/LICENSE.md`](./assets/data/LICENSE.md), which contains the Unlicense notice and links to [The Unlicense](https://unlicense.org/). The notice permits copying, modification, publication, use, sale and distribution for commercial or non-commercial purposes; attribution is not required, and the work is provided without warranty. This records the notice associated with the word list; it does not claim provenance over any separately sourced dictionary content that may be incorporated into it. |
| `scenes/units/cubey/dialogues.txt` | Contains dialogue data used by the Cubey character system, organised into categories and A1–C2 rank levels, with lines and format placeholders. All dialogue was written by the developer. No third-party contributions have been identified. |

No other standalone dictionary or word-list file is present in the project.
