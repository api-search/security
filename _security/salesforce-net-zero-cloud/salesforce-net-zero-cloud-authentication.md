---
api_key_in: []
api_specs:
- filename: salesforce-net-zero-cloud-rest-api-openapi.yml
  format: yaml
  label: Net Zero Cloud REST API
  slug: net-zero-cloud-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-net-zero-cloud/refs/heads/main/openapi/salesforce-net-zero-cloud-rest-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Salesforce Net Zero Cloud Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Salesforce Net Zero Cloud secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Salesforce Net Zero Cloud
provider_slug: salesforce-net-zero-cloud
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  sources:
  - openapi/salesforce-net-zero-cloud-rest-api-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/salesforce-net-zero-cloud-rest-api-openapi.yml
  type: http
slug: salesforce-net-zero-cloud-authentication
source_filename: salesforce-net-zero-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesforce-net-zero-cloud-rest-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n    scopes: 1\n  sources:\n  - openapi/salesforce-net-zero-cloud-rest-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/salesforce-net-zero-cloud-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-net-zero-cloud/refs/heads/main/authentication/salesforce-net-zero-cloud-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Carbon Accounting
- Carbon Emissions
- Climate
- Environmental
- ESG
- Net Zero
- Sustainability
---
