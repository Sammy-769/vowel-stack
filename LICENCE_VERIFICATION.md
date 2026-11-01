# Vowel Stack — Licence Verification Checklist

This checklist records issues not conclusively resolved by the project files. A checked box means evidence has been gathered and reviewed; none are pre-checked. Do not describe an item as commercially cleared until the applicable rights and licence conditions are verified.

## Audio — 17 files

- [ ] For each audio file listed in the **Audio** table of [ASSET_CREDITS.md](./ASSET_CREDITS.md), locate the original download, purchase, commission, or creation record. Confirm the current filename, any earlier filename, creator/source, exact licence, and permitted commercial/game redistribution.
- [ ] Specifically verify `assets/audio/game/freeze.mp3` against original records. The project does not establish that it was originally called `freeze-sound.mp3`.
- [ ] If any sound came from Pixabay or another stock library, recover the original asset page, author, download date, applicable licence version, and evidence of the licence terms at download time. No Pixabay match is established by this project inventory.

## Images and graphics — 58 files

- [ ] Review **all 58 image/graphic rows** in the **Images and graphics** table of [ASSET_CREDITS.md](./ASSET_CREDITS.md). Obtain per-file source/creation records and verify commercial use, modification, redistribution, and attribution requirements.
- [ ] Confirm the creator and rights for all game artwork, icons, splash art, and game icon; no source or applicable image licence is established by the project files.
- [ ] Check whether any artwork is AI-generated with the creator or original source records. Metadata and appearance inspected here do not establish AI origin.
- [ ] Confirm the original source and licence for `assets/sprite/game sprite/grabill54-good-13724_512.gif`. Its embedded Photoshop metadata identifies editing software only.
- [ ] Confirm source and reuse rights for `assets/sprite/crypto address/ton.png` and `assets/sprite/crypto address/usdt(TRC20).png`; screenshot metadata is not a licence.
- [ ] Obtain image-asset licence terms for SilentWolf's five bundled graphics under `addons/silent_wolf/assets/gfx/`, separately from the plugin-code licence.

## Fonts — 10 files

- [ ] For `assets/fonts/DynaPuff/DynaPuff-VariableFont_wdth,wght.ttf`, `assets/fonts/Fredoka/Fredoka-Medium.ttf`, `assets/fonts/Gluten/Gluten-Medium.ttf`, `assets/fonts/Rubik_Bubbles/RubikBubbles-Regular.ttf`, and `assets/fonts/Sniglet/Sniglet-ExtraBold.ttf`, confirm each included SIL OFL 1.1 notice applies to the exact binary and follow the licence's notice/redistribution requirements.
- [ ] Resolve the malformed upstream URL in `assets/fonts/Rubik_Bubbles/OFL.txt`; verify the correct Rubik Bubbles source independently.
- [ ] For `assets/fonts/FreeCheese_Font_1_0/FreeCheese-Regular.ttf`, `assets/fonts/Rainbow2000_Font_v1_04/Rainbow2000-Bold.ttf`, `assets/fonts/scabber-font/Scabber-q2Mn0.ttf`, and `assets/fonts/type-light-sans-font/TypeLightSans-KV84p.otf`, obtain source/creator evidence linking the font to the included CC0 1.0 text. The generic CC0 legal text alone does not establish that the specific font was dedicated under CC0.
- [ ] Obtain the source and font licence for `addons/silent_wolf/assets/fonts/Comfortaa-Bold.ttf`; no font-specific notice was found in the project.

## Language resources and licence-file scope

- [ ] Identify the source, compiler/author, and dataset licence for `assets/data/words_list.txt` (370,105 entries), including any restrictions inherited from the included words or source corpus.
- [ ] Confirm whether `assets/data/LICENSE.md` was intended to cover `words_list.txt` and identify the author/work to which that Unlicense dedication applies. Its presence in the same directory does not by itself establish the word list's provenance or rights.
- [ ] Confirm the author/ownership and any third-party contributions in `scenes/units/cubey/dialogues.txt`.

## Plugin, services, and release handover

- [ ] Obtain authoritative licensing, source/version provenance, and redistribution permission for the SilentWolf 0.9.9 addon under `addons/silent_wolf/`; no plugin licence file was found in the project.
- [ ] Confirm SilentWolf account/project ownership, service terms, any plan or payment requirements, and an approved account/data migration or buyer-owned replacement. Do not transfer seller credentials.
- [ ] Confirm rights and account ownership for the Effective CPM Network smartlink configured in `scripts/ad_manager.gd`; assess privacy/consent disclosures and replace the link if it is seller-controlled. The configured opaque identifier is intentionally omitted from these documents.
- [ ] Confirm or replace the Discord invite destination and review the Google connectivity-check request for the buyer's distribution and privacy disclosures.
- [ ] Verify applicable notices for the exact Godot Engine/export-template and Jolt-enabled engine build used in the delivered game.
- [ ] Review generated Android output and copied assets in `android/build/` before distribution; ensure build artifacts do not contain seller-owned signing credentials, account details, or other non-transferable configuration.

## Evidence to retain

For each completed item, retain the original asset page or receipt, creator/source identity, licence text/version and date, attribution requirements, and any permission or transfer correspondence. Keep credentials and private account information out of this checklist and any buyer-facing public materials.
