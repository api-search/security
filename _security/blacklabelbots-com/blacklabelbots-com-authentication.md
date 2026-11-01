---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for Ace API uses an API key sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Blacklabelbots Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: blacklabelbots-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: blacklabelbots-com
provider_slug: blacklabelbots-com
scheme_count: 1
schemes:
- evidence: 'Streamable HTTP at https://tryacee.com/mcp with Authorization: Bearer <key> , or the URL-only form https://tryacee.com/mcp/k/<key> .'
  header: Authorization
  how_to_obtain: Generate a key in the Ace dashboard; the key is shown once and must be stored securely.
  location: header
  name: Authorization
  type: http-bearer
slug: blacklabelbots-com-authentication
source_filename: blacklabelbots-com-authentication.yml
source_heading: Authentication Profile
source_url: https://tryacee.com/developers?utm_source=blacklabelbots.com&utm_medium=developers&utm_campaign=platform-20261016#keys
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://tryacee.com/developers?utm_source=blacklabelbots.com&utm_medium=developers&utm_campaign=platform-20261016#keys\nsources:\n- https://tryacee.com/developers?utm_source=blacklabelbots.com&utm_medium=developers&utm_campaign=platform-20261016#keys\n- https://blacklabelbots.com/marketing-setup\n- https://blacklabelbots.com/academy/niches__ai-chatbot-setup\n- https://blacklabelbots.com/academy/niches__tv-mounting\ndescription: Authentication for Ace API uses an API key sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Streamable HTTP at https://tryacee.com/mcp with Authorization: Bearer <key> , or the URL-only form https://tryacee.com/mcp/k/<key>\n    .'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a key in the Ace dashboard; the key is shown once and must be stored securely.\ndocs:\
  \ https://tryacee.com/developers?utm_source=blacklabelbots.com&utm_medium=developers&utm_campaign=platform-20261016#keys\n"
source_yaml_url: https://artifacts.apis.io/blacklabelbots-com/authentication/blacklabelbots-com-authentication.yml
summary_line: 1 scheme
tags:
- Business
- Software
- Productivity
- Automation
- Mac
- Windows
---
