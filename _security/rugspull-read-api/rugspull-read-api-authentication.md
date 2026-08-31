---
api_key_in: []
api_specs:
- filename: rugspull-read-api-indexer-api-openapi.yml
  format: yaml
  label: Rugspull Read API Indexer API
  slug: rugspull-read-api-indexer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rugspull-read-api/refs/heads/main/openapi/rugspull-read-api-indexer-api-openapi.yml
- filename: rugspull-read-api-market-api-openapi.yml
  format: yaml
  label: Rugspull Read API Market API
  slug: rugspull-read-api-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rugspull-read-api/refs/heads/main/openapi/rugspull-read-api-market-api-openapi.yml
- filename: rugspull-read-api-objects-api-openapi.yml
  format: yaml
  label: Rugspull Read API Objects API
  slug: rugspull-read-api-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rugspull-read-api/refs/heads/main/openapi/rugspull-read-api-objects-api-openapi.yml
- filename: rugspull-read-api-rugs-api-openapi.yml
  format: yaml
  label: Rugspull Read API Rugs API
  slug: rugspull-read-api-rugs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rugspull-read-api/refs/heads/main/openapi/rugspull-read-api-rugs-api-openapi.yml
- filename: rugspull-read-api-service-api-openapi.yml
  format: yaml
  label: Rugspull Read API Service API
  slug: rugspull-read-api-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rugspull-read-api/refs/heads/main/openapi/rugspull-read-api-service-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Rugspull Read Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rugspull Read API declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Rugspull Read API
provider_slug: rugspull-read-api
scheme_count: 0
schemes: []
slug: rugspull-read-api-authentication
source_filename: rugspull-read-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: https://rugspull.com/.well-known/api-onboarding\ndocs: https://github.com/pqchase/rugspull/blob/main/docs/INTEGRATION.md\nspec_source: openapi/rugspull-read-api-openapi.yml\nsummary: >-\n  The Rugspull Read API is fully anonymous. The OpenAPI 3.1 document declares no\n  components.securitySchemes and no root or per-operation security requirement, and\n  the provider's own API Onboarding descriptor states auth \"none\" and account\n  required false in machine-readable form. This is a deliberate, documented absence\n  rather than an undocumented one: the API is GET-only over a rebuildable public\n  cache, so there is no principal to authenticate and nothing to authorize.\nmodel: none\nschemes: []\nsecurity_requirement_declared: false\naccount_required: false\nregistration_required: false\napi_key_required: false\nagent_policy: allowed\nagent_policy_source: https://rugspull.com/.well-known/api-onboarding\ncredentials: []\nscopes:\n\
  \  model: none\n  note: >-\n    No authorization scopes exist. The provider states this explicitly in the\n    onboarding descriptor: \"No authorization scopes exist because this descriptor\n    covers read-only public cache endpoints only.\" scopes/ is intentionally absent.\ncors:\n  enabled: true\n  allow_origin: '*'\n  allow_methods: [GET, POST, OPTIONS]\n  allow_headers: [authorization, content-type, cf-turnstile-response, x-turnstile-token]\n  expose_headers: [link]\n  max_age: 86400\n  observed: 'live response headers on GET https://rugspull.com/api/rugs, 2026-08-11'\n  note: >-\n    The CORS preflight advertises POST and the Turnstile headers even though every\n    published operation is a GET. Those headers belong to the write surface the\n    Worker serves for the app itself (creation/upload flows behind /ops and /account/,\n    both Disallowed in robots.txt); they are not part of the published read contract.\nsettlement_boundary: >-\n  Wallets sign financial actions on BNB Smart\
  \ Chain directly. The API never buys,\n  sells, rugs, claims, refunds, or signs a transaction on a user's behalf, so no\n  delegated-authority or consent model is required for the published surface.\ngaps:\n  - No OAuth 2.0, OpenID Connect, or API-key surface exists to document.\n  - >-\n    Because access is anonymous and unmetered, there is no per-caller identity to\n    attach a rate limit, quota, or abuse policy to — see rate-limits/.\ncross_links:\n  conventions: conventions/rugspull-read-api-conventions.yml\n  well_known: well-known/rugspull-read-api-well-known.yml\n  rate_limits: rate-limits/rugspull-read-api-rate-limits.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rugspull-read-api/refs/heads/main/authentication/rugspull-read-api-authentication.yml
summary_line: 0 schemes
tags:
- bnb-smart-chain
- bsc
- wbnb
- Read Only
- OpenAPI
- high-risk
- discovery-cache
- DeFi
- Web3
- crypto-market-data
- indexer
---
