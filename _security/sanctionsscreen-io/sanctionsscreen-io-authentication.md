---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Sanctionsscreen Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: sanctionsscreen-io declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: sanctionsscreen-io
provider_slug: sanctionsscreen-io
scheme_count: 2
schemes:
- description: Scoped API keys with `cs_live_` prefix, per-tool scopes.
  in: header
  name: cs_live_*
  type: apiKey
- description: OAuth 2.1 planned (auth-code + PKCE, client-credentials, PRM, DCR).
  type: oauth2
slug: sanctionsscreen-io-authentication
source_filename: sanctionsscreen-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://sanctionsscreen.io/llms.txt\nschemes:\n  - type: apiKey\n    name: cs_live_*\n    in: header\n    description: Scoped API keys with `cs_live_` prefix, per-tool scopes.\n  - type: oauth2\n    description: OAuth 2.1 planned (auth-code + PKCE, client-credentials, PRM, DCR).\n"
source_yaml_url: https://artifacts.apis.io/sanctionsscreen-io/authentication/sanctionsscreen-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Sanctions
- Compliance
- API
- FinTech
---
