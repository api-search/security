---
anonymous_access: false
api_key_in: []
api_specs:
- filename: goodrecmovies-com-api-openapi.json
  format: json
  label: goodrecmovies public API API
  slug: goodrecmovies-public-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodrecmovies-com/openapi/_original/goodrecmovies-com-api-openapi.json
auth_types: []
description: goodrecmovies supports anonymous reads by default and an optional Agent API key sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: goodrecmovies Authentication
name_suffix: Authentication
oauth_flows: []
overview: goodrecmovies declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: goodrecmovies
provider_slug: goodrecmovies-com
scheme_count: 1
schemes:
- evidence: 'Agent API key (optional). `Authorization: Bearer grm_…` on /ask, /a2a, /mcp, /mcp/docs, /api/list, /api/search: 600 req/min and 100,000 requests per 30 days per account, shared by up to 5 active keys.'
  header: Authorization
  how_to_obtain: Keys are bought by humans at https://goodrecmovies.com/premium (Dodo checkout) and minted/revoked there.
  location: header
  name: Agent API key
  type: http-bearer
slug: goodrecmovies-com-authentication
source_filename: goodrecmovies-com-authentication.yml
source_heading: Authentication Profile
source_url: https://goodrecmovies.com/auth.md
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://goodrecmovies.com/auth.md\nsources:\n- https://goodrecmovies.com/auth.md\ndescription: goodrecmovies supports anonymous reads by default and an optional Agent API key sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Agent API key\n  evidence: 'Agent API key (optional). `Authorization: Bearer grm_…` on /ask, /a2a, /mcp, /mcp/docs, /api/list, /api/search: 600 req/min and 100,000\n    requests per 30 days per account, shared by up to 5 active keys.'\n  location: header\n  header: Authorization\n  how_to_obtain: Keys are bought by humans at https://goodrecmovies.com/premium (Dodo checkout) and minted/revoked there.\nnote: There is no OAuth flow, no client credentials, and no other authentication schemes.\ndocs: https://goodrecmovies.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/goodrecmovies-com/authentication/goodrecmovies-com-authentication.yml
summary_line: 1 scheme
tags:
- Movies
- Entertainment
- Recommendations
- Free
---
