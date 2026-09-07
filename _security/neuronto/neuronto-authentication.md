---
anonymous_access: true
api_key_in: []
api_specs:
- filename: neuronto-openapi.json
  format: json
  label: Neuronto ARD Registry API
  slug: ard-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neuronto/refs/heads/main/openapi/neuronto-openapi.json
auth_types: []
description: The API, MCP server and A2A interface are all anonymous by default - "no key, no signup" is the product's stated posture, and the live MCP tools/list and REST endpoints answered unauthenticated probes on 2026-09-07. An optional API key exists purely to raise allowances and unlock domain-scoped features.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Neuronto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Neuronto ARD Registry declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Neuronto ARD Registry
provider_slug: neuronto
scheme_count: 2
schemes:
- scope: All search, publishing, console and data-feed endpoints, the MCP server and the A2A interface work with no credential at anonymous allowances.
  type: none
- delivery: Not documented publicly; the first-party CLI passes it as --key KEY. The OpenAPI declares no securitySchemes.
  grants: ~6x anonymous allowances, 30 days of rank history, unlogged searches, and the domain-scoped /private/entries surface (internal services visible only to that domain's key). Pro keys (contact) raise allowances ~5x further with metering readable at GET /me.
  obtained: Prove control of a domain with one DNS record via POST /claim then POST /claim/verify ("Verified" tier, free). The MCP server card declares authentication.required false with no schemes.
  required: false
  type: apiKey
slug: neuronto-authentication
source_filename: neuronto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://neuronto.com/pricing\nname: Neuronto Authentication Profile\ndescription: The API, MCP server and A2A interface are all anonymous by default -\n  \"no key, no signup\" is the product's stated posture, and the live MCP tools/list\n  and REST endpoints answered unauthenticated probes on 2026-09-07. An optional API\n  key exists purely to raise allowances and unlock domain-scoped features.\ndefault: anonymous\nschemes:\n- type: none\n  scope: All search, publishing, console and data-feed endpoints, the MCP server\n    and the A2A interface work with no credential at anonymous allowances.\n- type: apiKey\n  required: false\n  obtained: Prove control of a domain with one DNS record via POST /claim then\n    POST /claim/verify (\"Verified\" tier, free). The MCP server card declares\n    authentication.required false with no schemes.\n  delivery: Not documented publicly; the first-party CLI passes it as --key KEY.\n    The\
  \ OpenAPI declares no securitySchemes.\n  grants: ~6x anonymous allowances, 30 days of rank history, unlogged searches,\n    and the domain-scoped /private/entries surface (internal services visible only\n    to that domain's key). Pro keys (contact) raise allowances ~5x further with\n    metering readable at GET /me.\nnotes:\n- GET /me answers without a key, returning the free-tier allowances rather than an\n  error.\n- No OAuth/OIDC surface; /.well-known/oauth-authorization-server and\n  /openid-configuration both 404.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neuronto/refs/heads/main/authentication/neuronto-authentication.yml
summary_line: 2 schemes
tags:
- Agentic Resource Discovery
- ARD
- MCP
- A2A
- API Discovery
- Registry
---
