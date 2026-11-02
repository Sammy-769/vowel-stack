# Vowel Stack — Asset Credits and Inventory

## Scope and counting method

This inventory covers the unique source assets present in the project: **86 files** comprising 17 audio files, 10 font files, 57 image/graphic files, and 2 language/text resources. SilentWolf's bundled media is included in the font and image counts; the plugin itself is documented separately in [THIRD_PARTY_DEPENDENCIES.md](./THIRD_PARTY_DEPENDENCIES.md).

Godot import sidecars (`*.import`), the generated `.godot/` cache, and copies/build outputs under `android/build/` are not counted as separate assets. `android/build/` contains copies of some project resources as well as generated Android output. Licence/README files are documentation accompanying assets and are not counted as game assets.

“Original filename not identified” means the project contents do not establish an earlier filename. No source match is inferred from a descriptive filename. In particular, no project evidence identifies `freeze.mp3` as formerly named `freeze-sound.mp3`.

## Audio — 17 files

The audio files have MP3 or OGG content as indicated by their extensions and file signatures. Inspected readable ID3/Vorbis tags did not establish source or licence. The entries below distinguish developer-supplied source information from independently verified file provenance. A supplied asset-page URL identifies the claimed source but does not, by itself, prove that the project file is that download or that licence conditions were met. Commercial-use rights are not confirmed for any audio file.

### Pixabay sound effects

The developer supplied the following claimed source matches. “Claimed match” is not an independent content-level verification of the downloaded file.

| Game sound | Current project filename and location | Claimed original asset | Claimed source page | Licence reference and status |
|---|---|---|---|---|
| Victory | `assets/audio/game/victory.mp3` | Level Up 08 | [Pixabay asset page](https://pixabay.com/sound-effects/film-special-effects-level-up-08-402152/) | [Pixabay Content License Summary](https://pixabay.com/service/license-summary/) and [full terms](https://pixabay.com/service/terms/); applicability and compliance require confirmation |
| Freeze | `assets/audio/game/freeze.mp3` | Iced Magic 6 | [Pixabay asset page](https://pixabay.com/sound-effects/film-special-effects-iced-magic-6-378606/) | [Pixabay Content License Summary](https://pixabay.com/service/license-summary/) and [full terms](https://pixabay.com/service/terms/); applicability and compliance require confirmation |
| Notification | `assets/audio/game/notification.mp3` | New Notification 051 | [Pixabay asset page](https://pixabay.com/sound-effects/technology-new-notification-051-494246/) | [Pixabay Content License Summary](https://pixabay.com/service/license-summary/) and [full terms](https://pixabay.com/service/terms/); applicability and compliance require confirmation |
| Slow motion | `assets/audio/game/slow_motion.mp3` | Slowdown FX | [Pixabay asset page](https://pixabay.com/sound-effects/film-special-effects-slowdown-fx-343685/) | [Pixabay Content License Summary](https://pixabay.com/service/license-summary/) and [full terms](https://pixabay.com/service/terms/); applicability and compliance require confirmation |
| Money | `assets/audio/money/money.mp3` | Cashier "Ka-ching" Sound Effect | [Pixabay asset page](https://pixabay.com/sound-effects/film-special-effects-cashier-quotka-chingquot-sound-effect-129698/) | [Pixabay Content License Summary](https://pixabay.com/service/license-summary/) and [full terms](https://pixabay.com/service/terms/); applicability and compliance require confirmation |
| Error | `assets/audio/money/error.mp3` | UI Error Pop | [Pixabay asset page](https://pixabay.com/sound-effects/film-special-effects-ui-error-pop-515668/) | [Pixabay Content License Summary](https://pixabay.com/service/license-summary/) and [full terms](https://pixabay.com/service/terms/); applicability and compliance require confirmation |
| Pop | `assets/audio/pop/pop.mp3` | Pop | [Pixabay asset page](https://pixabay.com/sound-effects/film-special-effects-pop-402324/) | [Pixabay Content License Summary](https://pixabay.com/service/license-summary/) and [full terms](https://pixabay.com/service/terms/); applicability and compliance require confirmation |
| Balloon pop | `assets/audio/pop/balloon pop.mp3` | Balloon Pop Sound Effect | [Pixabay asset page](https://pixabay.com/sound-effects/film-special-effects-balloon-pop-sound-effect-504628/) | [Pixabay Content License Summary](https://pixabay.com/service/license-summary/) and [full terms](https://pixabay.com/service/terms/); applicability and compliance require confirmation |
| Pop select | `assets/audio/pop/pop_select.mp3` | Multi Pop 2 | [Pixabay asset page](https://pixabay.com/sound-effects/film-special-effects-multi-pop-2-188167/) | [Pixabay Content License Summary](https://pixabay.com/service/license-summary/) and [full terms](https://pixabay.com/service/terms/); applicability and compliance require confirmation |
| Platform | `assets/audio/platform/platform.mp3` | Body Fall | [Pixabay asset page](https://pixabay.com/sound-effects/film-special-effects-body-fall-142378/) | [Pixabay Content License Summary](https://pixabay.com/service/license-summary/) and [full terms](https://pixabay.com/service/terms/); applicability and compliance require confirmation |
| Platform 3 | `assets/audio/platform/platform3.mp3` | Heavy Body Fall | [Pixabay asset page](https://pixabay.com/sound-effects/film-special-effects-heavy-body-fall-352446/) | [Pixabay Content License Summary](https://pixabay.com/service/license-summary/) and [full terms](https://pixabay.com/service/terms/); applicability and compliance require confirmation |
| Platform 2 | `assets/audio/platform/platform2.mp3` | Character Fall Impact | [Pixabay asset page](https://pixabay.com/sound-effects/film-special-effects-character-fall-impact-352287/) | [Pixabay Content License Summary](https://pixabay.com/service/license-summary/) and [full terms](https://pixabay.com/service/terms/); applicability and compliance require confirmation |
| Reward | `assets/audio/game/reward.mp3` | Achievement Badge Pop Sound 1 | [Pixabay asset page](https://pixabay.com/sound-effects/film-special-effects-achievement-badge-pop-sound-1-547860/) | [Pixabay Content License Summary](https://pixabay.com/service/license-summary/) and [full terms](https://pixabay.com/service/terms/); applicability and compliance require confirmation |

The developer confirms that the two remaining unidentified sound effects were also downloaded from Pixabay. No individual asset page or original title has been identified for either file.

| Current project filename and location | Source information | Individual asset page | Licence reference and status |
|---|---|---|---|
| `assets/audio/game/combo.mp3` | Pixabay (developer-confirmed platform source) | Not yet identified | [Pixabay Content License Summary](https://pixabay.com/service/license-summary/); individual asset and compliance not independently verified |
| `assets/audio/money/coin.mp3` | Pixabay (developer-confirmed platform source) | Not yet identified | [Pixabay Content License Summary](https://pixabay.com/service/license-summary/); individual asset and compliance not independently verified |

### StockTune music

The developer supplied these StockTune source-page matches. StockTune is documented separately from Pixabay. The source pages identify the claimed tracks, but the project's audio files have not been independently matched to the downloads. StockTune's [Use License and Terms](https://stocktune.com/info/terms) state that its content is public domain and may be used, shared, and adapted without restrictions for personal and commercial purposes. The terms also ask users to act responsibly and ethically, prohibit implying endorsement without permission, and note that StockTune may not own or have created the content. The terms page was supplied by the developer; the underlying track rights and file-to-page matches still require confirmation.

| Game music | Current project filename and location | Claimed original asset | Claimed source page | Licence status |
|---|---|---|---|---|
| In-game music | `assets/audio/music/game_music.ogg` | Echoes of Childhood Dreams | [StockTune track page](https://stocktune.com/free-music/echoes-of-childhood-dreams-230054-140085) | [StockTune Use License and Terms](https://stocktune.com/info/terms) state public-domain use for personal and commercial purposes. Confirm this file matches the track and check underlying rights; StockTune says it may not own or have created supplied content. |
| Lobby music | `assets/audio/music/lobby_music.ogg` | Memories in Slow Motion | [StockTune track page](https://stocktune.com/free-music/memories-in-slow-motion-230053-140085) | [StockTune Use License and Terms](https://stocktune.com/info/terms) state public-domain use for personal and commercial purposes. Confirm this file matches the track and check underlying rights; StockTune says it may not own or have created supplied content. |

## Fonts — 10 files

The font binaries' embedded metadata identifies family/style for several fonts but does not itself establish licensing. Five font folders contain notices that state SIL Open Font License 1.1 and identify a project/author; the association of each notice with the exact bundled binary should still be confirmed. Four other font folders contain the text of CC0 1.0 but do not identify an author, source, or explicit dedication of that exact font to CC0. SilentWolf's official [FAQ](https://silentwolf.com/) answers “Can I use SilentWolf in a commercial game?” with “Yes! You can use SilentWolf in games that make money.” This confirms commercial-game use of SilentWolf; the FAQ does not give separate font-specific attribution or standalone redistribution terms for bundled assets.

| Current project filename and location | Source and licence evidence |
|---|---|---|
| `assets/fonts/DynaPuff/DynaPuff-VariableFont_wdth,wght.ttf` | `OFL.txt` names The DynaPuff Project Authors, states SIL OFL 1.1, and gives `https://github.com/googlefonts/dynapuff`. Confirm notice-to-binary association and compliance. |
| `assets/fonts/Fredoka/Fredoka-Medium.ttf` | `OFL.txt` names The Fredoka Project Authors, states SIL OFL 1.1, and gives `https://github.com/hafontia/Fredoka-One`. Confirm notice-to-binary association and compliance. |
| `assets/fonts/FreeCheese_Font_1_0/FreeCheese-Regular.ttf` | `License.txt` contains CC0 1.0 legal text, but does not identify this font as the work or name an affirmer/source. Licence applicability requires confirmation. |
| `assets/fonts/Gluten/Gluten-Medium.ttf` | `OFL.txt` names The Gluten Project Authors, states SIL OFL 1.1, and gives `https://github.com/Etcetera-Type-Co/Gluten`. Confirm notice-to-binary association and compliance. |
| `assets/fonts/Rainbow2000_Font_v1_04/Rainbow2000-Bold.ttf` | `License.txt` contains CC0 1.0 legal text, but does not identify this font as the work or name an affirmer/source. Licence applicability requires confirmation. |
| `assets/fonts/Rubik_Bubbles/RubikBubbles-Regular.ttf` | `OFL.txt` names The Rubik Filtered Project Authors and states SIL OFL 1.1. Its source URL is malformed as written (`https://https://github.com/NaN-xyz/Rubik-Filtered`); confirm the correct source and notice-to-binary association. |
| `assets/fonts/scabber-font/Scabber-q2Mn0.ttf` | `License-473a.txt` contains CC0 1.0 legal text, but does not identify this font as the work or name an affirmer/source. Licence applicability requires confirmation. |
| `assets/fonts/Sniglet/Sniglet-ExtraBold.ttf` | `OFL.txt` names Haley Fiege, Brenda Gallo, and Pablo Impallari and states SIL OFL 1.1. No source URL is supplied in the notice. Confirm notice-to-binary association and compliance. |
| `assets/fonts/type-light-sans-font/TypeLightSans-KV84p.otf` | `License-473a.txt` contains CC0 1.0 legal text, but does not identify this font as the work or name an affirmer/source. Licence applicability requires confirmation. |
| `addons/silent_wolf/assets/fonts/Comfortaa-Bold.ttf` | Bundled with SilentWolf. Its official [FAQ](https://silentwolf.com/) confirms that SilentWolf may be used in commercial games; this supports use of the bundled font as part of the addon in a commercial game. The FAQ does not specify the font's source, attribution requirements, or standalone redistribution terms if the font is separated from the addon. |

## Images and graphics — 57 files

The developer reports that most game graphics were generated using OpenAI ChatGPT's image-generation capabilities. Individual generation histories were not retained. The notes below therefore record the general reported source but do not claim that any specific listed file was individually verified as ChatGPT-generated. OpenAI's [Terms of Use](https://openai.com/policies/row-terms-of-use/) are the supplied reference; as reported by the developer, commercial use is generally permitted and attribution is not required, subject to the applicable terms. This does not establish the origin of a particular file or resolve third-party material potentially incorporated into output.

### Backgrounds and mode graphics — 11 files

| Current project filename and location | Source and licence evidence |
|---|---|
| `assets/sprite/background/bg1.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/background/bg2.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/background/bg3.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/background/bg4.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/background/bg5.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/background/endless icon.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/background/endless_tumb.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/background/levels icon.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/background/levels.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/background/levels_tumb.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/background/lobby.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |

### Interface buttons — 16 files

| Current project filename and location | Source and licence evidence |
|---|---|
| `assets/sprite/buttons/achievements.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/buttons/ad button.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/buttons/back button.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/buttons/daily word.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/buttons/discord.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/buttons/freeze.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/buttons/gift.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/buttons/home green.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/buttons/home red.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/buttons/leaderboard.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/buttons/nextlevel.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/buttons/pause button.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/buttons/platform drop.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/buttons/progress.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/buttons/slowmo.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/buttons/tryagain button.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |

### Gameplay objects and character parts — 9 files

| Current project filename and location | Source and licence evidence |
|---|---|
| `assets/sprite/game sprite/coin.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/game sprite/display podium.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/game sprite/frame.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/game sprite/land.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/game sprite/lava.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/game sprite/rock.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/game sprite/star.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/player/eyes.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/player/mouth.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |

### Cubey outfits — 8 files

| Current project filename and location | Source and licence evidence |
|---|---|
| `assets/sprite/outfits/birthday.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/outfits/cat ears.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/outfits/chef.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/outfits/crown.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/outfits/graduation cap.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/outfits/pirate.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/outfits/top hat.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/outfits/wizard.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |

### UI and project branding — 6 files

| Current project filename and location | Source and licence evidence |
|---|---|
| `assets/sprite/ui/adaptive_icon_background.svg` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/ui/adaptive_icon_foreground.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/ui/tryagain.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `assets/sprite/ui/victory.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `boot image.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |
| `gameicon.png` | Developer reports most game graphics were generated with ChatGPT; this file's individual origin is unverified. See OpenAI Terms of Use above. |

### Crypto-address graphics — 2 files

| Current project filename and location | Source and licence evidence |
|---|---|
| `assets/sprite/crypto address/ton.png` | Developer confirms this is a screenshot, not OpenAI-generated artwork. Its original source and reuse rights are unverified. Developer plans to remove it after the sale is confirmed; verify it is absent from the delivered project. |
| `assets/sprite/crypto address/usdt(TRC20).png` | Developer confirms this is a screenshot, not OpenAI-generated artwork. Its original source and reuse rights are unverified. Developer plans to remove it after the sale is confirmed; verify it is absent from the delivered project. |

### Bundled SilentWolf plugin graphics — 5 files

| Current project filename and location | Source and licence evidence |
|---|---|
| `addons/silent_wolf/assets/gfx/checkbox_checked.png` | Bundled with SilentWolf. Its official [FAQ](https://silentwolf.com/) confirms that SilentWolf may be used in commercial games; this supports use of the bundled graphic as part of the addon in a commercial game. The FAQ does not specify the graphic's source, attribution requirements, or standalone redistribution terms if it is separated from the addon. |
| `addons/silent_wolf/assets/gfx/checkbox_unchecked.png` | Bundled with SilentWolf. Its official [FAQ](https://silentwolf.com/) confirms that SilentWolf may be used in commercial games; this supports use of the bundled graphic as part of the addon in a commercial game. The FAQ does not specify the graphic's source, attribution requirements, or standalone redistribution terms if it is separated from the addon. |
| `addons/silent_wolf/assets/gfx/dummy_info_icon_small.png` | Bundled with SilentWolf. Its official [FAQ](https://silentwolf.com/) confirms that SilentWolf may be used in commercial games; this supports use of the bundled graphic as part of the addon in a commercial game. The FAQ does not specify the graphic's source, attribution requirements, or standalone redistribution terms if it is separated from the addon. |
| `addons/silent_wolf/assets/gfx/info_icon.png` | Bundled with SilentWolf. Its official [FAQ](https://silentwolf.com/) confirms that SilentWolf may be used in commercial games; this supports use of the bundled graphic as part of the addon in a commercial game. The FAQ does not specify the graphic's source, attribution requirements, or standalone redistribution terms if it is separated from the addon. |
| `addons/silent_wolf/assets/gfx/info_icon_small.png` | Bundled with SilentWolf. Its official [FAQ](https://silentwolf.com/) confirms that SilentWolf may be used in commercial games; this supports use of the bundled graphic as part of the addon in a commercial game. The FAQ does not specify the graphic's source, attribution requirements, or standalone redistribution terms if it is separated from the addon. |

## Language and dialogue resources — 2 files

| Current project filename and location | Purpose and source/licence evidence |
|---|---|
| `assets/data/words_list.txt` | 370,105 lines/entries used by the local word manager for dictionary validation. The associated licence text is in [`assets/data/LICENSE.md`](./assets/data/LICENSE.md), which contains the Unlicense notice and links to [The Unlicense](https://unlicense.org/). The notice permits copying, modification, publication, use, sale and distribution for commercial or non-commercial purposes; attribution is not required, and the work is provided without warranty. This records the notice associated with the word list, not the provenance of any separately sourced dictionary or dataset content that may be incorporated into it. The list's compiler/source and any such third-party content remain unverified. |
| `scenes/units/cubey/dialogues.txt` | Contains dialogue data used by the Cubey character system, organised into categories and A1–C2 rank levels, with lines and format placeholders. The developer confirms the dialogue was written entirely by the developer. No separate third-party source is reported. |

The project contains no other standalone dictionary or word-list file identified by this inventory.

## Evidence limitations

The project contains font notices and metadata and the Unlicense text at `assets/data/LICENSE.md`. It does not contain download receipts or individual ChatGPT image-generation records, or evidence matching the claimed Pixabay/StockTune audio pages to the actual downloaded files. StockTune's terms also caution that it may not own or have created its supplied content. Filenames, appearance, and a general source statement alone do not establish an individual asset's origin or applicable rights. See [LICENCE_VERIFICATION.md](./LICENCE_VERIFICATION.md) for the remaining checks.
