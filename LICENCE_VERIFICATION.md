# Vowel Stack — Licence Verification Checklist

This checklist tracks the asset and service items worth confirming during handover. Items are not pre-checked; tick them off as each is reviewed.

## Audio — 17 files

### Pixabay sound effects

- [ ] Retain the Pixabay Content License Summary and full terms applicable at download time alongside the delivered project. The [Summary](https://pixabay.com/service/license-summary/) and [full terms](https://pixabay.com/service/terms/) cover commercial use, modifications and redistribution as part of a game.
- [ ] Where download records are still available for the 13 named sound effects, keep them with the project so the source pages can be traced.
- [ ] For `assets/audio/game/combo.mp3` and `assets/audio/money/coin.mp3`, note that both came from Pixabay. No individual asset page is currently recorded.

### StockTune music

- [ ] Retain the [StockTune Use License and Terms](https://stocktune.com/info/terms) alongside the delivered project. The terms state that StockTune content is public domain and may be used, shared and adapted for personal and commercial purposes, and also ask for responsible and ethical use and prohibit implied endorsement.
- [ ] Keep the two track source pages on file: "Echoes of Childhood Dreams" and "Memories in Slow Motion".

## Images and graphics — 57 files

- [ ] The bulk of the game's graphics were generated with ChatGPT; OpenAI's [Terms of Use](https://openai.com/policies/row-terms-of-use/) assign the user OpenAI's rights in generated output to the extent permitted by law. Retain a copy of those terms with the delivery.
- [ ] `assets/sprite/crypto address/ton.png` and `assets/sprite/crypto address/usdt(TRC20).png` are screenshots, not AI-generated graphics. Confirm both have been deleted from the project before handover.
- [ ] The five graphics under `addons/silent_wolf/assets/gfx/` are bundled with SilentWolf. SilentWolf's official [FAQ](https://silentwolf.com/) confirms commercial-game use of the addon.

## Fonts — 10 files

- [ ] Keep the SIL OFL 1.1 notices that ship with DynaPuff, Fredoka, Gluten, Rubik Bubbles and Sniglet alongside the fonts. These notices name the project authors.
- [ ] Fix or annotate the malformed source URL in `assets/fonts/Rubik_Bubbles/OFL.txt`; the intended project is Rubik-Filtered on GitHub.
- [ ] The CC0 1.0 text in the FreeCheese, Rainbow2000, Scabber and TypeLightSans folders documents the licence terms distributed with those fonts. Keep those notices alongside the fonts.
- [ ] Comfortaa is bundled with SilentWolf; SilentWolf's FAQ covers commercial-game use of the addon.

## Language and dialogue resources

- [ ] `assets/data/LICENSE.md` contains the Unlicense text and should travel with `assets/data/words_list.txt`. Keep the notice with the delivered word list.
- [ ] `scenes/units/cubey/dialogues.txt` was written entirely by the developer. No third-party contributions have been identified.

## Plugin, services and release handover

- [ ] SilentWolf's official FAQ is the documented basis for using the plugin in a commercial game. Retain it with the delivery.
- [ ] Confirm SilentWolf account and project ownership, service terms, any plan or payment requirements, and arrange an approved account/data migration or a buyer-owned replacement. Do not transfer seller credentials.
- [ ] Remove the Effective CPM Network smartlink in `scripts/ad_manager.gd` after the sale is confirmed. Verify no seller-specific identifier remains in the delivered project.
- [ ] Remove the Discord invite link after the sale is confirmed. `assets/sprite/buttons/discord.png` is an AI-generated graphic and is unrelated to the external invite URL.
- [ ] Review the Google connectivity-check request in `scripts/ad_manager.gd` for the buyer's distribution and privacy disclosures.
- [ ] Check generated Android output and copied assets in `android/build/` before distribution to ensure no seller-owned signing credentials, account details or other non-transferable configuration are included.

## Evidence to retain

For each asset, keep the original page or receipt, creator/source identity, licence text and version, and any attribution requirements. Keep credentials out of this checklist and any buyer-facing materials.
