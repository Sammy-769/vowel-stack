# Vowel Stack — Licence Verification Checklist

This checklist records issues not conclusively resolved by the project files and the developer's confirmations. A checked box means evidence has been gathered and reviewed; none are pre-checked. Do not describe an item as commercially cleared until the applicable rights and licence conditions are verified.

## Audio — 17 files

- [ ] For the 15 audio files other than `game_music.ogg` and `lobby_music.ogg`, locate the original download, purchase, commission, or creation record. Confirm the current filename, creator/source, exact licence, and permitted commercial/game redistribution.
- [ ] Specifically verify `assets/audio/game/freeze.mp3` against original records. The project does not establish that it was originally called `freeze-sound.mp3`.
- [ ] Retain the original StockTune track pages or download records for `game_music.ogg` and `lobby_music.ogg`, if available. StockTune's published [Terms of Service](https://stocktune.com/info/terms) state that its content is public-domain content and may be used for personal and commercial purposes. StockTune also notes that it may not own or have created all content provided on its website.

## Images and graphics — 57 files currently

- [ ] After the sale is confirmed and before handover, delete `assets/sprite/crypto address/ton.png` and `assets/sprite/crypto address/usdt(TRC20).png`. Confirm that neither file remains in the delivered project or Android build output.
- [ ] After deleting those two screenshots, update the inventory count from 86 to 84 total files and from 57 to 55 image/graphic files.
- [ ] Retain available generation records for the 50 game artwork and UI graphics that the developer confirms were generated using OpenAI image-generation tools. Review the [OpenAI Terms of Use](https://openai.com/policies/row-terms-of-use/), including the user's responsibility for inputs and the possibility of non-unique outputs.
- [ ] Retain a dated copy or record of SilentWolf's [official FAQ](https://silentwolf.com/), which confirms that SilentWolf can be used in commercial games. The developer relies on this confirmation for commercial use of the bundled addon and its included resources.

## Fonts — 10 files

- [ ] For `assets/fonts/DynaPuff/DynaPuff-VariableFont_wdth,wght.ttf`, `assets/fonts/Fredoka/Fredoka-Medium.ttf`, `assets/fonts/Gluten/Gluten-Medium.ttf`, `assets/fonts/Rubik_Bubbles/RubikBubbles-Regular.ttf`, and `assets/fonts/Sniglet/Sniglet-ExtraBold.ttf`, confirm each included SIL OFL 1.1 notice applies to the exact binary and follow the licence's notice/redistribution requirements.
- [ ] Resolve the malformed upstream URL in `assets/fonts/Rubik_Bubbles/OFL.txt`; verify the correct Rubik Bubbles source independently.
- [ ] For `assets/fonts/FreeCheese_Font_1_0/FreeCheese-Regular.ttf`, `assets/fonts/Rainbow2000_Font_v1_04/Rainbow2000-Bold.ttf`, `assets/fonts/scabber-font/Scabber-q2Mn0.ttf`, and `assets/fonts/type-light-sans-font/TypeLightSans-KV84p.otf`, obtain source/creator evidence linking the font to the included CC0 1.0 text. The generic CC0 legal text alone does not establish that the specific font was dedicated under CC0.
- [ ] Retain a dated copy or record of SilentWolf's [official FAQ](https://silentwolf.com/) as evidence of permission to use SilentWolf in commercial games, including its bundled resources.

## Language resources and licence-file scope

- [ ] Identify the source, compiler/author, and dataset licence for `assets/data/words_list.txt` (370,105 entries), including any restrictions inherited from the included words or source corpus.
- [ ] Confirm whether `assets/data/LICENSE.md` was intended to cover `words_list.txt` and identify the author/work to which that Unlicense dedication applies. Its presence in the same directory does not by itself establish the word list's provenance or rights.

Developer confirmation: `scenes/units/cubey/dialogues.txt` was written entirely by the developer. No third-party contributions have been identified.

## Plugin, services, engine notices, and release handover

- [ ] Retain a dated copy or record of SilentWolf's [official FAQ](https://silentwolf.com/), which confirms that SilentWolf can be used in commercial games and that credit is not required. No formal plugin licence file was found in the bundled addon. The FAQ does not expressly set out source-code transfer or service-account migration terms.
- [ ] Confirm SilentWolf account/project ownership, service terms, any plan or payment requirements, and an approved account/data migration or buyer-owned replacement. Do not transfer seller credentials.
- [ ] After the sale is confirmed and before handover, remove the Effective CPM Network smartlink and its associated code/configuration from `scripts/ad_manager.gd`. Test that the game no longer opens or references the seller's smartlink.
- [ ] After the sale is confirmed and before handover, remove the seller's Discord invitation URL. Check that no game action opens the removed invitation. Decide whether the Discord button should be removed or repurposed.
- [ ] Include the Godot Engine MIT copyright notice and licence statement when distributing Godot engine binaries or an exported game that contains them. Check the notices supplied with the exact engine build for any third-party components.
- [ ] Review generated Android output and copied assets in `android/build/` before distribution; ensure build artefacts do not contain seller-owned signing credentials, account details, or other non-transferable configuration.

## Evidence to retain

For each completed item, retain the original asset page or receipt, creator/source identity, licence text/version and date, attribution requirements, and any permission or transfer correspondence. Keep credentials and private account information out of this checklist and any buyer-facing public materials.
