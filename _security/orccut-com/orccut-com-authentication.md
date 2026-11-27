---
anonymous_access: false
api_key_in: []
auth_types: []
description: Orccut uses bearer tokens for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Orccut Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orccut declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Orccut
provider_slug: orccut-com
scheme_count: 1
schemes:
- evidence: Bearer tokens minted for your agents stay valid across logins — nothing to re-paste into a client config.
  header: Authorization
  how_to_obtain: Mint a token via the UI at /ui/tokens and paste it into your client.
  location: header
  name: Bearer token
  type: http-bearer
slug: orccut-com-authentication
source_filename: orccut-com-authentication.yml
source_heading: Authentication Profile
source_url: https://orccut.com/auth/login
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://orccut.com/auth/login\nsources:\n- https://orccut.com/auth/login\n- https://orccut.com/auth/register\ndescription: Orccut uses bearer tokens for authentication.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: Bearer tokens minted for your agents stay valid across logins — nothing to re-paste into a client config.\n  location: header\n  header: Authorization\n  how_to_obtain: Mint a token via the UI at /ui/tokens and paste it into your client.\ndocs: https://orccut.com/auth/login\n"
source_yaml_url: https://artifacts.apis.io/orccut-com/authentication/orccut-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Video Editing
- AI Integration
- MCP Server
- Media
- OpenAPI
---
