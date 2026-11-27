---
anonymous_access: false
api_key_in: []
auth_types: []
description: Lawgical uses a single OAuth authentication flow. No API keys or static bearer tokens are supported.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Lawgical Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lawgical declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Lawgical
provider_slug: lawgical-vn
scheme_count: 1
schemes:
- evidence: 'There is one authentication path: **OAuth**.'
  how_to_obtain: User authorizes in a browser window on Lawgical's login page; the client uses PKCE with the public client ID `lawgical-mcp` (no client secret).
  name: OAuth
  type: oauth2
slug: lawgical-vn-authentication
source_filename: lawgical-vn-authentication.yml
source_heading: Authentication Profile
source_url: https://lawgical.vn/llms-full.txt
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://lawgical.vn/llms-full.txt\nsources:\n- https://lawgical.vn/llms-full.txt\n- https://lawgical.vn/cai-dat\ndescription: Lawgical uses a single OAuth authentication flow. No API keys or static bearer tokens are supported.\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: 'There is one authentication path: **OAuth**.'\n  how_to_obtain: User authorizes in a browser window on Lawgical's login page; the client uses PKCE with the public client ID `lawgical-mcp` (no\n    client secret).\ndocs: https://lawgical.vn/llms-full.txt\n"
source_yaml_url: https://artifacts.apis.io/lawgical-vn/authentication/lawgical-vn-authentication.yml
summary_line: 1 scheme
tags:
- Law
- Artificial Intelligence
- Legal Tech
- Vietnam
---
