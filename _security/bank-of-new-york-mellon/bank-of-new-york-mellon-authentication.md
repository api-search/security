---
api_key_in: []
api_specs:
- filename: bny-mellon-treasury-services-api-openapi.yml
  format: yaml
  label: BNY Mellon Treasury Services API
  slug: treasury-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-new-york-mellon/refs/heads/main/openapi/bny-mellon-treasury-services-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Bank Of New York Mellon Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: BNY Mellon secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: BNY Mellon
provider_slug: bank-of-new-york-mellon
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 5
    tokenUrl: https://api.bnymellon.com/oauth/token
  name: OAuth2
  sources:
  - openapi/bny-mellon-treasury-services-api-openapi.yml
  type: oauth2
slug: bank-of-new-york-mellon-authentication
source_filename: bank-of-new-york-mellon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bny-mellon-treasury-services-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.bnymellon.com/oauth/token\n    scopes: 5\n  sources:\n  - openapi/bny-mellon-treasury-services-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-of-new-york-mellon/refs/heads/main/authentication/bank-of-new-york-mellon-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Asset Servicing
- Banking
- Institutional Banking
- Payments
- Treasury
- Wire Transfers
- Fortune 500
---
