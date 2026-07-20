---
api_key_in: []
api_specs:
- filename: even-financial-openapi-original.json
  format: json
  label: Engine by MoneyLion API
  slug: engine-by-moneylion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/even-financial/refs/heads/main/openapi/even-financial-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Even Financial Authentication
name_suffix: Authentication
oauth_flows: []
overview: Even Financial secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Even Financial
provider_slug: even-financial
scheme_count: 3
schemes:
- description: A publishable bearer token, safe to ship in application/client code and downloaded to a user's device. Restricted access — only non-sensitive endpoints (e.g. lead submission, UI utilities).
  name: publishableBearerToken
  scheme: bearer
  sources:
  - openapi/even-financial-openapi-original.json
  type: http
- description: A confidential bearer token that must be managed like a password and kept server-side. Grants access to sensitive endpoints (analytics, payouts, full lead data).
  name: confidentialBearerToken
  scheme: bearer
  sources:
  - openapi/even-financial-openapi-original.json
  type: http
- description: A bearer token scoped to experimental / early-access endpoints.
  name: experimentalBearerToken
  scheme: bearer
  sources:
  - openapi/even-financial-openapi-original.json
  type: http
slug: even-financial-authentication
source_filename: even-financial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/even-financial-openapi-original.json\ndocs: https://engine.tech/docs/api-reference/\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  notes: >-\n    All requests to the Engine by MoneyLion (formerly Even Financial) API are authenticated\n    with a bearer token in the Authorization header, prefixed with \"Bearer \". Tokens are two\n    UUIDs concatenated with an underscore. There are two production token classes plus an\n    experimental class; there is no OAuth 2.0 / OpenID Connect flow.\nschemes:\n- name: publishableBearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    A publishable bearer token, safe to ship in application/client code and downloaded to a\n    user's device. Restricted access — only non-sensitive endpoints (e.g. lead submission,\n    UI utilities).\n  sources:\n  - openapi/even-financial-openapi-original.json\n- name: confidentialBearerToken\n  type: http\n  scheme: bearer\n\
  \  description: >-\n    A confidential bearer token that must be managed like a password and kept server-side.\n    Grants access to sensitive endpoints (analytics, payouts, full lead data).\n  sources:\n  - openapi/even-financial-openapi-original.json\n- name: experimentalBearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    A bearer token scoped to experimental / early-access endpoints.\n  sources:\n  - openapi/even-financial-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/even-financial/refs/heads/main/authentication/even-financial-authentication.yml
summary_line: http · 3 schemes
tags:
- Company
- Financial Services
- Embedded Finance
- Fintech
- Lending
- Personal Loans
- Credit Cards
- Marketplace
- Recommendation Engine
- Lead Generation
---
