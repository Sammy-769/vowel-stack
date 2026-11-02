# Vowel Stack — Third-Party Dependencies and Services

This inventory is based on the project files inspected. It does not assume that any developer account, service subscription, advertising account, data, or URL configuration will transfer with a sale.

## Bundled plugin and libraries

| Dependency | Location / evidence | Purpose | Licence, account, and transfer notes |
|---|---|---|---|
| SilentWolf Godot plugin, version 0.9.9 (`plugin.cfg` credits Brass Harpooner) | `addons/silent_wolf/`; enabled in `project.godot`. Game code calls SilentWolf for scores and player data. The plugin also includes account/authentication scenes and code. | Online leaderboards and cloud player data; bundled code also implements player account/authentication features. | SilentWolf's official [FAQ](https://silentwolf.com/) answers “Can I use SilentWolf in a commercial game?” with “Yes! You can use SilentWolf in games that make money.” This confirms commercial-game use of SilentWolf. The bundled addon contains no separate licence file or source repository URL; the FAQ does not specify standalone redistribution/transfer terms for the plugin's bundled fonts and graphics. Confirm any applicable addon/asset transfer terms, plus current service/account requirements. The plugin calls `api.silentwolf.com`; confirm whether the buyer needs a new game/project registration, credentials, subscription, or data migration. Do not assume the seller's account or existing data transfers. |
| Godot Engine and its Android export artifacts | `project.godot` declares Godot feature version `4.7`; `android/build/` contains generated `godot-lib.template_debug.aar`, `godot-lib.template_release.aar`, and a Gradle wrapper JAR. | Game runtime and Android build/export support. | No separate app-specific Android plugin/library was identified in the inspected build output. The engine/export-template versions and their applicable notices should be confirmed for the delivered build. Android build output is generated material, not proof of transferable tool accounts or release credentials. |
| Jolt physics engine integration | `project.godot` selects `Jolt Physics` as the 3D physics engine. No separate Jolt plugin/library was identified in the project. | Physics engine setting. | Appears to be an engine-level integration rather than a separately bundled project dependency. Verify applicable engine/distribution notices for the exact engine build used. |

## External services and links

| Service | Project evidence and use | Buyer considerations |
|---|---|---|
| SilentWolf cloud API | SilentWolf plugin code calls `api.silentwolf.com`; game scripts use score and player-data APIs. | Requires confirmation of the service's current terms, account/project ownership, pricing or plan requirements, and transfer/migration process. A seller-owned account or game registration is not assumed to transfer. |
| SilentWolf multiplayer WebSocket endpoints | Plugin code in `addons/silent_wolf/Multiplayer/` and `addons/silent_wolf/Muliplayer/` refers to `ws.silentwolfmp.com`. The game's lobby button currently shows a “coming soon” panel, and no game-level call to the plugin's multiplayer API was found. | This appears to be bundled plugin capability rather than an active game service integration. Confirm with the vendor before enabling it; service terms and account requirements are unverified. |
| Effective CPM Network smartlink | `scripts/ad_manager.gd` defines a smartlink on `effectivecpmnetwork.com` and opens it externally. No separate ad SDK/library was identified. | The configured link contains an opaque identifier, intentionally not reproduced here. Verify account ownership, authorization to use/transfer it, current network terms, payout arrangements, user-consent/privacy disclosures, and suitability for the buyer's release. The buyer may need to replace it with a buyer-controlled link. |
| Google connectivity-check endpoint | `scripts/ad_manager.gd` references `connectivitycheck.gstatic.com/generate_204` for connectivity checking. | A network request to a Google-operated endpoint; no Google SDK or account dependency was identified. Review whether the request is needed and the applicable privacy disclosures. |
| Discord | The game lobby opens an external Discord invite link. | This is a link, not a bundled SDK. The invite destination/community and any associated account are not presumed to transfer; confirm or replace it for the buyer. The invitation token is omitted. |

## Other findings

- The only project addon enabled in `project.godot` is `res://addons/silent_wolf/plugin.cfg`. No other plugin directory was found under `addons/`.
- No separately declared third-party game library or app-specific Android AAR/JAR was identified. The Android build folder includes the Godot engine AARs and Gradle wrapper artifacts noted above.
- The project contains generated `.godot/` cache data and `android/build/` output, including copied game resources. These are not additional unique source assets or proof of service/account rights.
- Service or account identifiers and opaque configured link values are deliberately not reproduced in this document. Review them securely before transfer; do not publish seller credentials.

## Handover actions

1. Retain the SilentWolf FAQ statement permitting commercial-game use. Confirm any separate plugin and bundled-asset redistribution/transfer terms, and obtain current service terms.
2. Decide whether the buyer will use a new SilentWolf project/account and arrange any necessary data migration without transferring seller credentials.
3. Confirm, remove, or replace the configured ad smartlink under an account controlled by the buyer; assess privacy, consent, advertising, and payout terms.
4. Confirm or replace the Discord invite link and connectivity-check behavior for the buyer's release.
5. Confirm the Godot engine/export-template version and include all applicable third-party notices for the delivered build.

For unresolved asset source and licence questions, see [LICENCE_VERIFICATION.md](./LICENCE_VERIFICATION.md).
