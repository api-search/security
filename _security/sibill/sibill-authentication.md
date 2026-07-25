---
api_key_in: []
api_specs:
- filename: sibill-account-api-openapi.yml
  format: yaml
  label: Sibill Account API
  slug: sibill-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-account-api-openapi.yml
- filename: sibill-category-api-openapi.yml
  format: yaml
  label: Sibill Category API
  slug: sibill-category-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-category-api-openapi.yml
- filename: sibill-company-api-openapi.yml
  format: yaml
  label: Sibill Company API
  slug: sibill-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-company-api-openapi.yml
- filename: sibill-counterpart-api-openapi.yml
  format: yaml
  label: Sibill Counterpart API
  slug: sibill-counterpart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-counterpart-api-openapi.yml
- filename: sibill-document-api-openapi.yml
  format: yaml
  label: Sibill Document API
  slug: sibill-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-document-api-openapi.yml
- filename: sibill-documentsectional-api-openapi.yml
  format: yaml
  label: Sibill DocumentSectional API
  slug: sibill-documentsectional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-documentsectional-api-openapi.yml
- filename: sibill-flow-api-openapi.yml
  format: yaml
  label: Sibill Flow API
  slug: sibill-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-flow-api-openapi.yml
- filename: sibill-payment-api-openapi.yml
  format: yaml
  label: Sibill Payment API
  slug: sibill-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-payment-api-openapi.yml
- filename: sibill-product-api-openapi.yml
  format: yaml
  label: Sibill Product API
  slug: sibill-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-product-api-openapi.yml
- filename: sibill-reconciliation-api-openapi.yml
  format: yaml
  label: Sibill Reconciliation API
  slug: sibill-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-reconciliation-api-openapi.yml
- filename: sibill-subcategory-api-openapi.yml
  format: yaml
  label: Sibill Subcategory API
  slug: sibill-subcategory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-subcategory-api-openapi.yml
- filename: sibill-transaction-api-openapi.yml
  format: yaml
  label: Sibill Transaction API
  slug: sibill-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-transaction-api-openapi.yml
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
