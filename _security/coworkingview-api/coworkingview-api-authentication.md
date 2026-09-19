---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coworkingview-api-config-api-openapi.yml
  format: yaml
  label: CoworkingView API Config API
  slug: coworkingview-api-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/openapi/coworkingview-api-config-api-openapi.yml
- filename: coworkingview-api-facets-api-openapi.yml
  format: yaml
  label: CoworkingView API Facets API
  slug: coworkingview-api-facets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/openapi/coworkingview-api-facets-api-openapi.yml
- filename: coworkingview-api-geo-api-openapi.yml
  format: yaml
  label: CoworkingView API Geo API
  slug: coworkingview-api-geo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/openapi/coworkingview-api-geo-api-openapi.yml
- filename: coworkingview-api-health-api-openapi.yml
  format: yaml
  label: CoworkingView API Health API
  slug: coworkingview-api-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/openapi/coworkingview-api-health-api-openapi.yml
- filename: coworkingview-api-leads-api-openapi.yml
  format: yaml
  label: CoworkingView API Leads API
  slug: coworkingview-api-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/openapi/coworkingview-api-leads-api-openapi.yml
- filename: coworkingview-api-market-api-openapi.yml
  format: yaml
  label: CoworkingView API Market API
  slug: coworkingview-api-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/openapi/coworkingview-api-market-api-openapi.yml
- filename: coworkingview-api-operators-api-openapi.yml
  format: yaml
  label: CoworkingView API Operators API
  slug: coworkingview-api-operators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/openapi/coworkingview-api-operators-api-openapi.yml
- filename: coworkingview-api-places-api-openapi.yml
  format: yaml
  label: CoworkingView API Places API
  slug: coworkingview-api-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/openapi/coworkingview-api-places-api-openapi.yml
- filename: coworkingview-api-properties-api-openapi.yml
  format: yaml
  label: CoworkingView API Properties API
  slug: coworkingview-api-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/openapi/coworkingview-api-properties-api-openapi.yml
- filename: coworkingview-api-rankings-api-openapi.yml
  format: yaml
  label: CoworkingView API Rankings API
  slug: coworkingview-api-rankings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/openapi/coworkingview-api-rankings-api-openapi.yml
- filename: coworkingview-api-search-api-openapi.yml
  format: yaml
  label: CoworkingView API Search API
  slug: coworkingview-api-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/openapi/coworkingview-api-search-api-openapi.yml
auth_types: []
description: 'The CoworkingView /v1 REST API declares no security schemes: every GET under /v1 is unauthenticated (no API key, client ID or session). The two write paths (POST /v1/leads/inquiry, POST /v1/leads/contact) are not gated by an agent credential either — they are gated by a Cloudflare Turnstile challenge token, returning CHALLENGE_FAILED (403) when it is missing or invalid. The provider publishes an auth.md agent skill that states this plainly.'
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Coworkingview Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoworkingView API declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: CoworkingView API
provider_slug: coworkingview-api
scheme_count: 0
schemes: []
slug: coworkingview-api-authentication
source_filename: coworkingview-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: CoworkingView Authentication\ndescription: >-\n  The CoworkingView /v1 REST API declares no security schemes: every GET under /v1 is unauthenticated (no API\n  key, client ID or session). The two write paths (POST /v1/leads/inquiry, POST /v1/leads/contact) are not\n  gated by an agent credential either — they are gated by a Cloudflare Turnstile challenge token, returning\n  CHALLENGE_FAILED (403) when it is missing or invalid. The provider publishes an auth.md agent skill that\n  states this plainly.\ngenerated: '2026-09-15'\nmethod: searched\nsource: >-\n  openapi/coworkingview-api-openapi.json (components.securitySchemes is empty; no top-level security) plus the\n  provider's own https://coworkingview.com/auth.md (HTTP 200, text/markdown) and the\n  /.well-known/oauth-protected-resource document (scopes_supported and bearer_methods_supported both empty).\nschemes: []\nprofile:\n  reads:\n    auth: none\n    detail: All GET /v1/* operations (properties, search, facets,\
  \ market rates, rankings, operators, places, health, config) are public. No WWW-Authenticate is emitted on any response.\n  writes:\n    auth: turnstile-challenge\n    detail: POST /v1/leads/inquiry and POST /v1/leads/contact require a Cloudflare Turnstile challengeToken in the request body in production; absence/invalidity yields 403 with code CHALLENGE_FAILED. This is bot mitigation, not an agent credential.\noauth:\n  present: false\n  note: >-\n    oauth-authorization-server and openid-configuration documents resolve on coworkingview.com but declare no\n    grant types, scopes or bearer methods; their agent_auth.skill points back at auth.md, which states OAuth\n    client registration/token issuance is \"not applicable\" for this API.\ndocs: https://coworkingview.com/auth.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coworkingview-api/refs/heads/main/authentication/coworkingview-api-authentication.yml
summary_line: 0 schemes
tags:
- Co-Working
- Flexible Workspace
- Real-Estate
- Location Services
- Search
- Comparison
- MCP
- agent-native
- Business
---
