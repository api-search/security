---
api_key_in: []
api_specs:
- filename: landing-public-openapi.json
  format: json
  label: Landing Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landing/refs/heads/main/openapi/landing-public-openapi.json
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Landing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Landing secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Landing
provider_slug: landing
scheme_count: 0
schemes: []
slug: landing-authentication
source_filename: landing-authentication.yml
source_heading: Authentication Profile
source_url: https://www.hellolanding.com/.well-known/mcp/server-card.json
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.hellolanding.com/.well-known/mcp/server-card.json\nsources:\n- https://www.hellolanding.com/.well-known/mcp/server-card.json\n- https://www.hellolanding.com/api/public\n- https://www.hellolanding.com/llms.txt\n- openapi/landing-public-openapi.json\ndocs: https://www.hellolanding.com/api/public\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  authentication_required: false\nschemes: []\nmodel:\n  type: none\n  detail: >-\n    Landing's public surface is deliberately unauthenticated. The MCP server\n    card records auth.type \"none\" (\"Unauthenticated, read-only. Rate limits may\n    apply.\"), the OpenAPI declares no components.securitySchemes and no\n    top-level security, the REST reference states \"No auth.\", and the embedded\n    schema.org Service block carries authenticationRequired = \"false\".\n  verified: >-\n    Live unauthenticated calls to /api/public/markets, /api/public/search\
  \ and\n    /api/public/status returned 200 on 2026-07-19.\nscope:\n  public_surface: >-\n    Read-only catalog access — markets, filters, search, home detail,\n    flex options, quotes, market info, policy FAQ, status.\n  boundary: >-\n    Reservation completion and payment are not exposed. Anything under /api/\n    other than /api/public is disallowed to bots in robots.txt and is not part\n    of the public contract. No authenticated/partner API is publicly documented.\noauth_scopes: null\noauth_scopes_note: >-\n  No OAuth surface exists, so no scopes/ artifact is produced for this provider\n  (per the OAuth-only rule in the enrichment contract).\ncross_ref: conventions/landing-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landing/refs/heads/main/authentication/landing-authentication.yml
summary_line: none · 0 schemes
tags:
- Company
- Proptech
- Real Estate
- Rentals
- Furnished Apartments
- Corporate Housing
- Travel
- Agent Native
- MCP
- Search
---
