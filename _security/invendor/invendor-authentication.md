---
api_key_in: []
api_specs:
- filename: invendor-common-openapi-original.json
  format: json
  label: Invendor Common API
  slug: invendor-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invendor/refs/heads/main/openapi/invendor-common-openapi-original.json
- filename: invendor-reporting-openapi-original.json
  format: json
  label: Invendor Reporting API
  slug: invendor-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invendor/refs/heads/main/openapi/invendor-reporting-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Invendor Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Invendor secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Invendor
provider_slug: invendor
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://identity.scanbro.com/connect/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://identity.scanbro.com/connect/token
  name: OAuth2
  sources:
  - openapi/invendor-common-openapi-original.json
  - openapi/invendor-reporting-openapi-original.json
  type: oauth2
slug: invendor-authentication
source_filename: invendor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/invendor-common-openapi-original.json, openapi/invendor-reporting-openapi-original.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://identity.scanbro.com/connect/authorize\n    tokenUrl: https://identity.scanbro.com/connect/token\n    scopes: 1\n  sources:\n  - openapi/invendor-common-openapi-original.json\n  - openapi/invendor-reporting-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/invendor/refs/heads/main/authentication/invendor-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Inventory Management
- Vendor Managed Inventory
- Industrial Vending
- Supply Chain
- Warehouse Management
- Asset Tracking
---
