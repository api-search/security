---
api_key_in: []
api_specs:
- filename: affirm-transactions-api-openapi.yml
  format: yaml
  label: Affirm Transactions API
  slug: affirm-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/openapi/affirm-transactions-api-openapi.yml
- filename: affirm-authorization-api-openapi.yml
  format: yaml
  label: Affirm Authorization API
  slug: affirm-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/openapi/affirm-authorization-api-openapi.yml
- filename: affirm-cards-api-openapi.yml
  format: yaml
  label: Affirm Cards API
  slug: affirm-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/openapi/affirm-cards-api-openapi.yml
- filename: affirm-checkouts-api-openapi.yml
  format: yaml
  label: Affirm Checkouts API
  slug: affirm-checkouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/openapi/affirm-checkouts-api-openapi.yml
- filename: affirm-disputes-api-openapi.yml
  format: yaml
  label: Affirm Disputes API
  slug: affirm-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/openapi/affirm-disputes-api-openapi.yml
- filename: affirm-promos-api-openapi.yml
  format: yaml
  label: Affirm Promos API
  slug: affirm-promos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/openapi/affirm-promos-api-openapi.yml
- filename: affirm-settlement-events-api-openapi.yml
  format: yaml
  label: Affirm Settlement Events API
  slug: affirm-settlement-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/openapi/affirm-settlement-events-api-openapi.yml
- filename: affirm-transaction-events-api-openapi.yml
  format: yaml
  label: Affirm Transaction Events API
  slug: affirm-transaction-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/openapi/affirm-transaction-events-api-openapi.yml
- filename: affirm-transactions-api-openapi.yml
  format: yaml
  label: Affirm Transactions API
  slug: affirm-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/openapi/affirm-transactions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Affirm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Affirm secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Affirm
provider_slug: affirm
scheme_count: 1
schemes:
- description: HTTP Basic Authentication using the merchant's public API key as the username and private API key as the password, Base64-encoded as per RFC 7617.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/affirm-checkout-openapi.yml
  - openapi/affirm-direct-api-openapi.yml
  - openapi/affirm-disputes-openapi.yml
  - openapi/affirm-transactions-openapi.yml
  type: http
slug: affirm-authentication
source_filename: affirm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/affirm-checkout-openapi.yml, openapi/affirm-direct-api-openapi.yml, openapi/affirm-disputes-openapi.yml,\n  openapi/affirm-transactions-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using the merchant's public API key as the username\n    and private API key as the password, Base64-encoded as per RFC 7617.\n  sources:\n  - openapi/affirm-checkout-openapi.yml\n  - openapi/affirm-direct-api-openapi.yml\n  - openapi/affirm-disputes-openapi.yml\n  - openapi/affirm-transactions-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/authentication/affirm-authentication.yml
summary_line: http · 1 scheme
tags:
- Fintech
- BNPL
- Lending
- Payments
- Consumer
---
