---
api_key_in: []
api_specs:
- filename: sibill-openapi-original.json
  format: json
  label: Sibill Integration API
  slug: sibill-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Sibill Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sibill secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sibill
provider_slug: sibill
scheme_count: 1
schemes:
- description: The Sibill Integration API authenticates every request with an API key sent as a Bearer token in the Authorization header, over HTTPS only. Keys are issued separately per environment (Development vs Production).
  format: Bearer ${api_key}
  header: Authorization
  in: header
  name: authorization
  scheme: bearer
  sources:
  - openapi/sibill-openapi-original.json
  type: http
slug: sibill-authentication
source_filename: sibill-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.sibill.com/api-reference/\nspec: openapi/sibill-openapi-original.json\ndocs: https://docs.sibill.com/\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\nschemes:\n- name: authorization\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: \"Bearer ${api_key}\"\n  description: >-\n    The Sibill Integration API authenticates every request with an API key sent as\n    a Bearer token in the Authorization header, over HTTPS only. Keys are issued\n    separately per environment (Development vs Production).\n  sources:\n  - openapi/sibill-openapi-original.json\nnotes: >-\n  Upgraded from the OpenAPI-derived profile: the published spec declares the\n  scheme with an invalid `type: https`; the docs make clear it is standard HTTP\n  Bearer (RFC 6750) API-key auth. No OAuth/OIDC and no scope surface, so scopes/\n  is intentionally omitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/authentication/sibill-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Invoicing
- Payments
- Reconciliation
- Accounting
- Banking
- SME
- Open Banking
- Electronic Invoicing
- Italy
---
