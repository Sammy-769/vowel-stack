# Vowel Stack — Third-Party Dependencies and Services

This inventory is based on the project files and does not assume that any developer account, subscription, advertising account, data or URL configuration will transfer with the sale.

## Bundled plugin and libraries

| Dependency | Location / evidence | Purpose | Licence, account and transfer notes |
|---|---|---|---|
| SilentWolf Godot plugin, version 0.9.9 (`plugin.cfg` credits Brass Harpooner) | `addons/silent_wolf/`; enabled in `project.godot`. Game code calls SilentWolf for scores and player data. The plugin also includes account/authentication scenes and code. | Online leaderboards and cloud player data; bundled code also implements player account/authentication features. | SilentWolf's official [FAQ](https://silentwolf.com/) answers "Can I use SilentWolf in a commercial game?" with "Yes! You can use SilentWolf in games that make money." No separate plugin licence file is shipped in the addon. The plugin calls `api.silentwolf.com`; the seller's account and data do not transfer automatically. |

## External services and links

| Service | Project evidence and use | Buyer considerations |
|---|---|---|
| SilentWolf cloud API | SilentWolf plugin code calls `api.silentwolf.com`; game scripts use score and player-data APIs. | Requires its own SilentWolf account/project. The seller's account and cloud data do not transfer. |
| SilentWolf multiplayer WebSocket endpoints | Plugin code in `addons/silent_wolf/Multiplayer/` and `addons/silent_wolf/Muliplayer/` refers to `ws.silentwolfmp.com`. The in-game lobby button currently shows a "coming soon" panel; no game-level call to the plugin's multiplayer API was found. | Bundled plugin capability rather than an active integration. Check with the vendor before enabling. |
| Effective CPM Network smartlink | `scripts/ad_manager.gd` defines a smartlink on `effectivecpmnetwork.com` and opens it externally. | To be removed after the sale is confirmed. Verify that both the link and seller-specific opaque identifier are removed before delivery. |
| Google connectivity-check endpoint | `scripts/ad_manager.gd` references `connectivitycheck.gstatic.com/generate_204` for connectivity checking. | A network request to a Google-operated endpoint. No Google SDK or account dependency. |
| Discord | The game lobby opens an external Discord invite link. | A link, not a bundled SDK. The invite will be removed after the sale is confirmed. The `assets/sprite/buttons/discord.png` graphic is AI-generated and unrelated to the external invite. |

## Other findings

- The only project addon enabled in `project.godot` is `res://addons/silent_wolf/plugin.cfg`. No other plugin directory exists under `addons/`.
- No other project plugin or separately declared third-party game library was identified beyond the SilentWolf addon and the external services above.
- The project contains generated `.godot/` cache data and `android/build/` output, including copied game resources. These are not unique source assets.

## Handover actions

1. Retain SilentWolf's official FAQ as the documented basis for commercial-game use. The buyer will need their own SilentWolf account/project; arrange any necessary data migration without transferring seller credentials.
2. After the sale is confirmed, remove the Effective CPM Network smartlink and verify no seller-specific identifier remains in the delivered project.
3. After the sale is confirmed, remove the Discord invite link and verify the seller's invite destination is absent from the delivered project.
4. Review the Google connectivity-check behaviour for the buyer's release and related privacy disclosures.

For asset sources and licences, see [ASSET_CREDITS.md](./ASSET_CREDITS.md). For the remaining handover checks, see [LICENCE_VERIFICATION.md](./LICENCE_VERIFICATION.md).
