---
anonymous_access: false
api_key_in: []
auth_types: []
description: Apiauto Space uses a single API key authentication scheme.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Apiauto Space Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apiauto Space declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Apiauto Space
provider_slug: apiauto-space
scheme_count: 1
schemes:
- evidence: Every data request sends the key in the `X-API-Key` header.
  header: X-API-Key
  how_to_obtain: Open the bot @apiautospace_bot in Telegram, press Start, and the key is sent in a message.
  location: header
  name: X-API-Key
  type: apiKey
slug: apiauto-space-authentication
source_filename: apiauto-space-authentication.yml
source_heading: Authentication Profile
source_url: https://apiauto.space/en/docs/auth.md
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://apiauto.space/en/docs/auth.md\nsources:\n- https://apiauto.space/en/docs/auth.md\n- https://apiauto.space/docs/auth/\n- https://apiauto.space/en/docs/auth/\n- https://apiauto.space/en/docs/\ndescription: Apiauto Space uses a single API key authentication scheme.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Every data request sends the key in the `X-API-Key` header.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Open the bot @apiautospace_bot in Telegram, press Start, and the key is sent in a message.\nnote: No other authentication methods (OAuth, http-bearer, etc.) are documented on the provided pages.\ndocs: https://apiauto.space/en/docs/auth.md\n"
source_yaml_url: https://artifacts.apis.io/apiauto-space/authentication/apiauto-space-authentication.yml
summary_line: 1 scheme
tags:
- Used Cars
- Car Importers
- Dealers
- Price Trackers
- Auctions
---
