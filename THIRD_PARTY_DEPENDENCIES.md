# Vowel Stack — Third-Party Dependencies and Services

This inventory is based on the project files inspected and the developer's confirmations. It does not assume that any developer account, service subscription, advertising account, data, or URL configuration will transfer with a sale.

## Bundled plugin and libraries

| Dependency | Location / evidence | Purpose | Licence, account, and transfer notes |
|---|---|---|---|
| SilentWolf Godot plugin, version 0.9.9 (`plugin.cfg` credits Brass Harpooner) | `addons/silent_wolf/`; enabled in `project.godot`. Game code calls SilentWolf for scores and player data. The plugin also includes account/authentication scenes and code. | Online leaderboards and cloud player data; bundled code also implements player account/authentication features. | SilentWolf's [official FAQ](https://silentwolf.com/) explicitly confirms that SilentWolf can be used in commercial games, including games that make money. The developer relies on this confirmation for commercial use of the bundled addon and its included resources. No separate formal plugin licence file was found in the bundled addon. The FAQ does not expressly address source-code transfer, service-account migration, or data transfer. The plugin calls `api.silentwolf.com`. The buyer should use a buyer-owned account/project if required; do not transfer seller credentials or assume that the seller's account or existing data transfers. |

## External services and links

| Service | Project evidence and use | Buyer considerations |
|---|---|---|
| SilentWolf cloud API | SilentWolf plugin code calls `api.silentwolf.com`; game scripts use score and player-data APIs. | Requires confirmation of the service's current terms, account/project ownership, pricing or plan requirements, and transfer/migration process. A seller-owned account or game registration is not assumed to transfer. |
| SilentWolf multiplayer WebSocket endpoints | Plugin code in `addons/silent_wolf/Multiplayer/` and `addons/silent_wolf/Muliplayer/` refers to `ws.silentwolfmp.com`. The game's lobby button currently shows a "coming soon" panel, and no game-level call to the plugin's multiplayer API was found. | This appears to be bundled plugin capability rather than an active game service integration. Confirm with the vendor before enabling it; service terms and account requirements are unverified. |
| Effective CPM Network smartlink | `scripts/ad_manager.gd` currently defines a smartlink on `effectivecpmnetwork.com` and opens it externally. No separate ad SDK/library was identified. | Temporary seller-controlled integration. It is scheduled for removal after the sale is confirmed and before project handover. It is not included as a transferable service or account. The configured opaque identifier is intentionally omitted. |
| Google connectivity-check endpoint | `scripts/ad_manager.gd` references `connectivitycheck.gstatic.com/generate_204` for connectivity checking. | A network request to a Google-operated endpoint; no Google SDK or account dependency was identified. Review whether the request is needed and the applicable privacy disclosures. |
| Discord | The game lobby currently opens an external Discord invitation link. | This is a link, not a bundled SDK. The seller's invitation URL is scheduled for removal after the sale is confirmed and before project handover. It is not included as a transferable community or account. The invitation token is omitted. |

## Engine licence and build notices

Godot Engine is open-source software distributed under the MIT licence and may be used commercially. The project declares Godot feature version `4.7`; this declaration should not be treated as proof of the exact editor/export-template build used.

When distributing Godot engine binaries or an exported game containing them, include the Godot copyright notice and licence statement as required by the MIT licence. See the [official Godot licence](https://godotengine.org/license) and [Godot's licence-compliance guidance](https://docs.godotengine.org/en/latest/about/complying_with_licenses.html).

The `android/build/` directory contains generated Godot Android AARs and build output. These are build artefacts, not separate app-specific dependencies or transferable accounts. Review the directory before handover and remove any signing credentials or other seller-specific configuration.

## Other findings

- The only project addon enabled in `project.godot` is `res://addons/silent_wolf/plugin.cfg`. No other plugin directory was found under `addons/`.
- No separately declared third-party game library or app-specific Android AAR/JAR was identified.
- The project contains generated `.godot/` cache data and `android/build/` output, including copied game resources. These are not additional unique source assets or proof of service/account rights.
- Service or account identifiers and opaque configured link values are deliberately not reproduced in this document. Review them securely before transfer; do not publish seller credentials.

## Handover actions

1. Retain a dated copy or record of SilentWolf's official FAQ as evidence of permission to use SilentWolf in a commercial game.
2. Arrange for the buyer to use a buyer-owned SilentWolf project/account if required; do not transfer seller credentials. Confirm any required service plan and whether data migration is available.
3. After the sale is confirmed and before handover, remove the Effective CPM Network smartlink and its associated code/configuration. Test that no seller-controlled smartlink remains.
4. After the sale is confirmed and before handover, remove the seller's Discord invitation URL. Check that no game action opens the removed invitation. Decide whether the Discord button should be removed or repurposed.
5. Include the Godot MIT copyright notice and licence statement with any distributed Godot engine binaries or exported game containing them.

For unresolved asset source and licence questions, see [LICENCE_VERIFICATION.md](./LICENCE_VERIFICATION.md).
