---
api_key_in: []
api_specs:
- filename: planomy-tax-data-tax-data-api-openapi.yml
  format: yaml
  label: Planomy Tax Data Tax Data API
  slug: planomy-tax-data-tax-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planomy-tax-data/refs/heads/main/openapi/planomy-tax-data-tax-data-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Planomy Tax Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: Planomy Tax Data declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Planomy Tax Data
provider_slug: planomy-tax-data
scheme_count: 0
schemes: []
slug: planomy-tax-data-authentication
source_filename: planomy-tax-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://planomy.net/data/\ndocs: https://planomy.net/data/\nsummary:\n  types: []\n  authentication_required: false\n  model: open-access\n  statement: >-\n    \"No key and no sign-up.\" — https://planomy.net/data/. Both endpoints are static JSON files served\n    anonymously over HTTPS; there is no credential of any kind to obtain, present, rotate or revoke.\nschemes: []\nverified:\n  - check: anonymous GET of https://planomy.net/tax-data/2026.json\n    result: 200 application/json\n    fetched: '2026-08-09'\n  - check: anonymous GET of https://planomy.net/tax-data/index.json\n    result: 200 application/json\n    fetched: '2026-08-09'\n  - check: OpenAPI securitySchemes\n    result: >-\n      empty — openapi/planomy-tax-data-openapi.yml declares no securitySchemes and sets `security: []`\n      on both operations, which is the accurate machine-readable statement of an open API.\nnotes:\n  - >-\n    Keyless is a deliberate\
  \ posture, not an omission: the underlying figures are US-federal\n    public-domain data and the licence statement invites reuse.\n  - >-\n    There is a separate, unrelated account system for the Planomy planner application itself\n    (optional sign-in for cloud sync and Plus billing, /app/). It does not gate the data endpoints and\n    exposes no documented API.\n  - >-\n    Because there is no credential, an agent needs no secret handling for this API — the only client\n    concerns are caching (ETag / If-None-Match) and polite request volume. See\n    conventions/planomy-tax-data-conventions.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planomy-tax-data/refs/heads/main/authentication/planomy-tax-data-authentication.yml
summary_line: 0 schemes
tags:
- Tax
- Finance
- Open Data
- retirement
- government
- personal-finance
- irs
- social-security
- medicare
- JSON
---
