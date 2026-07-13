---
api_key_in: []
api_specs:
- filename: awin-affiliate-openapi.yml
  format: yaml
  label: Awin Accounts API
  slug: awin-affiliate-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-openapi.yml
- filename: awin-affiliate-openapi.yml
  format: yaml
  label: Awin Transactions API
  slug: awin-affiliate-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-openapi.yml
- filename: awin-affiliate-openapi.yml
  format: yaml
  label: Awin Reports API
  slug: awin-affiliate-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-openapi.yml
- filename: awin-affiliate-openapi.yml
  format: yaml
  label: Awin Commission Groups API
  slug: awin-affiliate-commission-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-openapi.yml
- filename: awin-affiliate-openapi.yml
  format: yaml
  label: Awin Programmes API
  slug: awin-affiliate-programmes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Awin Affiliate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Awin secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Awin
provider_slug: awin-affiliate
scheme_count: 1
schemes:
- description: OAuth 2.0 user-level access token generated at ui.awin.com/awin-api and sent as an Authorization Bearer header. The Create Transactions API is the exception and uses an x-api-key header instead. Many endpoints also accept the token as an accessToken query parameter.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/awin-affiliate-openapi.yml
  type: http
slug: awin-affiliate-authentication
source_filename: awin-affiliate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/awin-affiliate-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 user-level access token generated at ui.awin.com/awin-api and sent\n    as an Authorization Bearer header. The Create Transactions API is the exception and uses\n    an x-api-key header instead. Many endpoints also accept the token as an accessToken query\n    parameter.\n  sources:\n  - openapi/awin-affiliate-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/authentication/awin-affiliate-authentication.yml
summary_line: http · 1 scheme
tags:
- Affiliate Marketing
- Advertising
- Publishers
- Advertisers
- Transactions
- Reporting
- Commissions
- Performance Marketing
---
