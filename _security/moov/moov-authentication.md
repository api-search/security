---
api_key_in: []
api_specs:
- filename: moov-accounts-api-openapi.yml
  format: yaml
  label: Moov Accounts API
  slug: moov-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-accounts-api-openapi.yml
- filename: moov-authentication-api-openapi.yml
  format: yaml
  label: Moov Authentication API
  slug: moov-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-authentication-api-openapi.yml
- filename: moov-bank-accounts-api-openapi.yml
  format: yaml
  label: Moov Bank Accounts API
  slug: moov-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-bank-accounts-api-openapi.yml
- filename: moov-capabilities-api-openapi.yml
  format: yaml
  label: Moov Capabilities API
  slug: moov-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-capabilities-api-openapi.yml
- filename: moov-cards-api-openapi.yml
  format: yaml
  label: Moov Cards API
  slug: moov-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-cards-api-openapi.yml
- filename: moov-disputes-api-openapi.yml
  format: yaml
  label: Moov Disputes API
  slug: moov-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-disputes-api-openapi.yml
- filename: moov-payment-links-api-openapi.yml
  format: yaml
  label: Moov Payment Links API
  slug: moov-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-payment-links-api-openapi.yml
- filename: moov-payment-methods-api-openapi.yml
  format: yaml
  label: Moov Payment Methods API
  slug: moov-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-payment-methods-api-openapi.yml
- filename: moov-refunds-api-openapi.yml
  format: yaml
  label: Moov Refunds API
  slug: moov-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-refunds-api-openapi.yml
- filename: moov-representatives-api-openapi.yml
  format: yaml
  label: Moov Representatives API
  slug: moov-representatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-representatives-api-openapi.yml
- filename: moov-sweeps-api-openapi.yml
  format: yaml
  label: Moov Sweeps API
  slug: moov-sweeps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-sweeps-api-openapi.yml
- filename: moov-transfers-api-openapi.yml
  format: yaml
  label: Moov Transfers API
  slug: moov-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-transfers-api-openapi.yml
- filename: moov-wallets-api-openapi.yml
  format: yaml
  label: Moov Wallets API
  slug: moov-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-wallets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Moov Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moov secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Moov
provider_slug: moov
scheme_count: 1
schemes:
- description: OAuth2 bearer token obtained from the /oauth2/token endpoint. Include in the Authorization header as "Bearer {token}".
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/moov-api-openapi.yml
  type: http
slug: moov-authentication
source_filename: moov-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/moov-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth2 bearer token obtained from the /oauth2/token endpoint. Include in the\n    Authorization header as \"Bearer {token}\".\n  sources:\n  - openapi/moov-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/authentication/moov-authentication.yml
summary_line: http · 1 scheme
tags:
- Banking
- Embedded Finance
- Financial Infrastructure
- Money Movement
- Payments
- Transfers
---
