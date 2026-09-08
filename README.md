# Atropis / MC-ServerHost

Public project overview for the Atropis / MC-ServerHost free Minecraft hosting service and its modpack integrations.

- Hosting panel: https://free.mc-serverhost.net
- Website: https://mc-serverhost.net
- Maintainer: [LordTheFreak](https://github.com/LordTheFreak)

## Repository scope

This is a documentation-only repository. It is not the full hosting-panel source code or a deployable server package. It does not contain production configuration, credentials, private infrastructure details, player data, or modpack files.

## Project goal

Make Minecraft Java multiplayer hosting easier: users can discover a compatible modpack, select a specific version, review estimated resource requirements and create a server through a web panel backed by Pterodactyl.

## Current Modrinth integration

- On-demand modpack search, with popularity as the default sorting and additional search/sorting options.
- Version selection and compatibility checks for dedicated-server installation.
- Estimated RAM requirements and warnings when the user's available resources are insufficient.
- Integration with the free-hosting start queue, wake-on-join workflow and automatic shutdown after 20 minutes without players.

New packs and versions are discovered through provider searches rather than a fixed local list. A published client modpack is not automatically compatible with a dedicated server; availability depends on its files, loader/runtime requirements and compatibility checks. RAM figures are estimates unless an explicit author recommendation is available. Players need the matching client modpack version.

## Planned CurseForge integration

CurseForge support is being prepared and is not enabled. API access has not yet been approved.

The planned integration uses the official API for project discovery, version metadata and author-authorized server-pack downloads. It will respect authors' distribution choices, link to original project pages and avoid public file mirrors or workarounds for disabled third-party downloads. API credentials will remain server-side. Provider approval and successful server-pack compatibility checks are prerequisites for installation.

This repository does not imply approval, endorsement or affiliation by CurseForge, Overwolf, Modrinth, Mojang or Microsoft.

## Funding and author attribution

The free hosting service is financed through voluntary donations and advertising. Modpack and mod authors retain their rights. The planned CurseForge integration will credit the original projects and provide links to their project pages and available support links.

## Reporting issues

Repository issues may be used for non-sensitive documentation feedback. Do not post passwords, API keys, private server addresses, player information or unredacted logs.
