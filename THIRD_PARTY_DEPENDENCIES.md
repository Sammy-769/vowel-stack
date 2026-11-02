# Vowel Stack — Third-Party Dependencies and Services

This inventory is based on the project files inspected. It does not assume that any developer account, service subscription, advertising account, data, or URL configuration will transfer with a sale.

## Bundled plugin and libraries

| Dependency | Location / evidence | Purpose | Licence, account, and transfer notes |
|---|---|---|---|
| SilentWolf Godot plugin, version 0.9.9 (`plugin.cfg` credits Brass Harpooner) | `addons/silent_wolf/`; enabled in `project.godot`. Game code calls SilentWolf for scores and player data. The plugin also includes account/authentication scenes and code. | Online leaderboards and cloud player data; bundled code also implements player account/authentication features. | SilentWolf's official [FAQ](https://silentwolf.com/) answers “Can I use SilentWolf in a commercial game?” with “Yes! You can use SilentWolf in games that make money.” This is the documented basis for using SilentWolf in this commercial game. No separate plugin licence file or source repository URL was found in the addon. Confirm current service/account requirements; do not assume the seller's account or data transfers. The plugin calls `api.silentwolf.com`. |

## External services and links

| Service | Project evidence and use | Buyer considerations |
|---|---|---|
| SilentWolf cloud API | SilentWolf plugin code calls `api.silentwolf.com`; game scripts use score and player-data APIs. | Requires confirmation of the service's current terms, account/project ownership, pricing or plan requirements, and transfer/migration process. A seller-owned account or game registration is not assumed to transfer. |
| SilentWolf multiplayer WebSocket endpoints | Plugin code in `addons/silent_wolf/Multiplayer/` and `addons/silent_wolf/Muliplayer/` refers to `ws.silentwolfmp.com`. The game's lobby button currently shows a “coming soon” panel, and no game-level call to the plugin's multiplayer API was found. | This appears to be bundled plugin capability rather than an active game service integration. Confirm with the vendor before enabling it; service terms and account requirements are unverified. |
| Effective CPM Network smartlink | `scripts/ad_manager.gd` defines a smartlink on `effectivecpmnetwork.com` and opens it externally. No separate ad SDK/library was identified. | The developer plans to remove this link after the sale is confirmed. Verify that the link and seller-specific opaque identifier are removed before delivery. If retained, confirm account ownership, authorisation, current terms, payout arrangements, user-consent/privacy disclosures and suitability for the buyer's release. |
| Google connectivity-check endpoint | `scripts/ad_manager.gd` references `connectivitycheck.gstatic.com/generate_204` for connectivity checking. | A network request to a Google-operated endpoint; no Google SDK or account dependency was identified. Review whether the request is needed and the applicable privacy disclosures. |
| Discord | The game lobby opens an external Discord invite link. | This is a link, not a bundled SDK. The developer plans to remove the invite after the sale is confirmed; verify it is absent before delivery. The invite destination/community and any associated account are not presumed to transfer. The invitation token is omitted. |

## Other findings

- The only project addon enabled in `project.godot` is `res://addons/silent_wolf/plugin.cfg`. No other plugin directory was found under `addons/`.
- No other project plugin or separately declared third-party game library was identified beyond the SilentWolf addon and external services listed above.
- The project contains generated `.godot/` cache data and `android/build/` output, including copied game resources. These are not additional unique source assets or proof of service/account rights.
- Service or account identifiers and opaque configured link values are deliberately not reproduced in this document. Review them securely before transfer; do not publish seller credentials.

## Handover actions

1. Retain SilentWolf's official FAQ as the documented basis for commercial-game use. Confirm current service/account requirements; do not assume seller accounts or cloud data transfer.
2. Decide whether the buyer will use a new SilentWolf project/account and arrange any necessary data migration without transferring seller credentials.
3. After the sale is confirmed, remove the Effective CPM Network smartlink and verify no seller-specific identifier remains in the delivered project. If the link is retained instead, confirm rights, privacy, consent, advertising and payout terms.
4. After the sale is confirmed, remove the Discord invite link and verify the seller's invite destination is absent from the delivered project.
5. Review the Google connectivity-check behavior for the buyer's release and related privacy disclosures.

For unresolved asset source and licence questions, see [LICENCE_VERIFICATION.md](./LICENCE_VERIFICATION.md).
