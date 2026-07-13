---
api_key_in: []
api_specs:
- filename: allianz-trade-payment-overdues.yaml
  format: yaml
  label: Allianz Trade Payment Overdues API
  slug: payment-overdues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/openapi/allianz-trade-payment-overdues.yaml
- filename: allianz-trade-company-grade.yaml
  format: yaml
  label: Allianz Trade Company Grade API
  slug: company-grade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/openapi/allianz-trade-company-grade.yaml
- filename: allianz-trade-claims.yaml
  format: yaml
  label: Allianz Trade Claims API
  slug: claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/openapi/allianz-trade-claims.yaml
- filename: allianz-trade-policy.yaml
  format: yaml
  label: Allianz Trade Policy API
  slug: policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/openapi/allianz-trade-policy.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Allianz Trade Online Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Allianz Trade secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Allianz Trade
provider_slug: allianz-trade-online
scheme_count: 1
schemes:
- description: OAuth2 client credentials for Allianz Trade API access
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://api.allianz-trade.com/oauth2/token
  name: OAuth2
  sources:
  - openapi/allianz-trade-claims.yaml
  - openapi/allianz-trade-company-grade.yaml
  - openapi/allianz-trade-payment-overdues.yaml
  - openapi/allianz-trade-policy.yaml
  type: oauth2
slug: allianz-trade-online-authentication
source_filename: allianz-trade-online-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/allianz-trade-claims.yaml, openapi/allianz-trade-company-grade.yaml, openapi/allianz-trade-payment-overdues.yaml,\n  openapi/allianz-trade-policy.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.allianz-trade.com/oauth2/token\n    scopes: 2\n  description: OAuth2 client credentials for Allianz Trade API access\n  sources:\n  - openapi/allianz-trade-claims.yaml\n  - openapi/allianz-trade-company-grade.yaml\n  - openapi/allianz-trade-payment-overdues.yaml\n  - openapi/allianz-trade-policy.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/authentication/allianz-trade-online-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Credit Insurance
- Insurance
- Risk Management
- Trade Credit
- E-Commerce
- Surety
---
