# Vowel Stack — Licence Verification Checklist

This checklist records issues not conclusively resolved by the project files. A checked box means evidence has been gathered and reviewed; none are pre-checked. Do not describe an item as commercially cleared until the applicable rights and licence conditions are verified.

## Audio — 17 files

- [ ] For each audio file listed in the **Audio** section of [ASSET_CREDITS.md](./ASSET_CREDITS.md), locate the original download record. Confirm the current file is the supplied source asset, whether it was renamed or modified, the creator/source, exact licence and version, and permitted commercial use and redistribution in a game.

### Pixabay sound effects

- [ ] For the 13 developer-supplied Pixabay page matches in [ASSET_CREDITS.md](./ASSET_CREDITS.md), compare each project file with its claimed original download and retain evidence of the match. The supplied URLs identify claimed sources; they do not independently prove a match.
- [ ] Review the [Pixabay Content License Summary](https://pixabay.com/service/license-summary/) and [full terms](https://pixabay.com/service/terms/) applicable to each download. Confirm the terms/version in force at download time, commercial use, modifications, redistribution as part of a game, any restrictions, and any required records or attribution. The general licence links do not establish that these specific files meet the conditions.
- [ ] For `assets/audio/game/combo.mp3` and `assets/audio/money/coin.mp3`, retain the developer confirmation that the platform source was Pixabay and seek the individual title/asset page and creator. Until found, keep the asset page marked **Not yet identified**; do not infer a title or creator.
- [ ] Specifically verify `assets/audio/game/freeze.mp3` against the supplied claimed page for “Iced Magic 6”. The project does not establish that it was formerly named `freeze-sound.mp3`.

### StockTune music

- [ ] For `assets/audio/music/game_music.ogg` (“Echoes of Childhood Dreams”) and `assets/audio/music/lobby_music.ogg` (“Memories in Slow Motion”), compare each file with its claimed StockTune download and retain evidence of the match.
- [ ] Retain and review the [StockTune Use License and Terms](https://stocktune.com/info/terms) applicable when downloaded. The terms text supplied for this review states that StockTune content is public domain and may be used, shared, and adapted for personal and commercial purposes; it also asks for responsible and ethical use, prohibits implying endorsement without permission, and says StockTune may not own or have created the supplied content. Confirm the terms/version and that this intended use is covered. Do not apply Pixabay terms to these tracks.
- [ ] Because StockTune says it may not own or have created the supplied content, retain any available evidence of the tracks' underlying rights and confirm the audio files match the claimed pages. Record any applicable download conditions, attribution wording, restrictions, and licence evidence.

## Images and graphics — 57 files

- [ ] Review the 57 image/graphic paths in [ASSET_CREDITS.md](./ASSET_CREDITS.md) against the delivery contents and retain per-file source/creation evidence where available. The inventory paths were compared with the current project files; there were no duplicate, missing, or nonexistent image paths.
- [ ] The developer reports that most game graphics were generated using OpenAI ChatGPT, but individual generation histories are unavailable. Confirm file origins where possible and do not attribute any image individually without evidence. Review the applicable [OpenAI Terms of Use](https://openai.com/policies/row-terms-of-use/); the developer reports that commercial use is generally permitted and attribution is not required under those terms. The general report does not establish that a specific image is an output or resolve third-party material potentially incorporated into output.
- [ ] Confirm source and reuse rights for `assets/sprite/crypto address/ton.png` and `assets/sprite/crypto address/usdt(TRC20).png`; screenshot metadata and the general ChatGPT statement do not establish these files' origin.
- [ ] SilentWolf's official [FAQ](https://silentwolf.com/) says SilentWolf may be used in games that make money, supporting use of its bundled graphics as part of the addon in a commercial game. If transferring any of the five graphics under `addons/silent_wolf/assets/gfx/` separately from the addon, confirm their source, attribution, and standalone redistribution terms.

## Fonts — 10 files

- [ ] For `assets/fonts/DynaPuff/DynaPuff-VariableFont_wdth,wght.ttf`, `assets/fonts/Fredoka/Fredoka-Medium.ttf`, `assets/fonts/Gluten/Gluten-Medium.ttf`, `assets/fonts/Rubik_Bubbles/RubikBubbles-Regular.ttf`, and `assets/fonts/Sniglet/Sniglet-ExtraBold.ttf`, confirm each included SIL OFL 1.1 notice applies to the exact binary and follow the licence's notice/redistribution requirements.
- [ ] Resolve the malformed upstream URL in `assets/fonts/Rubik_Bubbles/OFL.txt`; verify the correct Rubik Bubbles source independently.
- [ ] For `assets/fonts/FreeCheese_Font_1_0/FreeCheese-Regular.ttf`, `assets/fonts/Rainbow2000_Font_v1_04/Rainbow2000-Bold.ttf`, `assets/fonts/scabber-font/Scabber-q2Mn0.ttf`, and `assets/fonts/type-light-sans-font/TypeLightSans-KV84p.otf`, obtain source/creator evidence linking the font to the included CC0 1.0 text. The generic CC0 legal text alone does not establish that the specific font was dedicated under CC0.
- [ ] SilentWolf's official [FAQ](https://silentwolf.com/) says SilentWolf may be used in games that make money, supporting use of its bundled Comfortaa font as part of the addon in a commercial game. If transferring the font separately from the addon, confirm its source, attribution, and standalone redistribution terms; no font-specific notice was found in the project.

## Language and dialogue resources

- [ ] `assets/data/LICENSE.md` contains the Unlicense text and is documented with `assets/data/words_list.txt` in [ASSET_CREDITS.md](./ASSET_CREDITS.md). Retain available records confirming the notice applies to the delivered word-list work. Separately identify the compiler/source and any third-party dictionary or dataset incorporated into the 370,105-entry list; the notice does not establish rights to independently sourced material.
- [ ] The developer confirms `scenes/units/cubey/dialogues.txt` was written entirely by the developer. Retain any available authorship records and confirm no third-party contributions need separate treatment. No separate licence claim is made in this checklist.

## Plugin, services, and release handover

- [ ] Retain SilentWolf's FAQ statement permitting use in commercial games. Separately obtain source/version information and confirm redistribution/transfer terms for the SilentWolf 0.9.9 addon and its bundled assets under `addons/silent_wolf/`; the FAQ does not specify standalone component rights, and no plugin licence file was found in the project.
- [ ] Confirm SilentWolf account/project ownership, service terms, any plan or payment requirements, and an approved account/data migration or buyer-owned replacement. Do not transfer seller credentials.
- [ ] Confirm rights and account ownership for the Effective CPM Network smartlink configured in `scripts/ad_manager.gd`; assess privacy/consent disclosures and replace the link if it is seller-controlled. The configured opaque identifier is intentionally omitted from these documents.
- [ ] Confirm or replace the Discord invite destination and review the Google connectivity-check request for the buyer's distribution and privacy disclosures.
- [ ] Verify applicable notices for the exact Godot Engine/export-template and Jolt-enabled engine build used in the delivered game.
- [ ] Review generated Android output and copied assets in `android/build/` before distribution; ensure build artifacts do not contain seller-owned signing credentials, account details, or other non-transferable configuration.

## Evidence to retain

For each completed item, retain the original asset page or receipt, creator/source identity, licence text/version and date, attribution requirements, and any permission or transfer correspondence. Keep credentials and private account information out of this checklist and any buyer-facing public materials.
