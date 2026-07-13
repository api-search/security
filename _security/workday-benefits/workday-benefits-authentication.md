---
api_key_in: []
api_specs:
- filename: Benefits.json
  format: json
  label: Workday Benefits API
  slug: workday-benefits-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Benefits/v40.2/Benefits.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Workday Benefits Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Workday Benefits secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Workday Benefits
provider_slug: workday-benefits
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token
  name: oauth2
  sources:
  - openapi/workday-benefits-openapi.yml
  type: oauth2
slug: workday-benefits-authentication
source_filename: workday-benefits-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-benefits-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token\n    scopes: 1\n  sources:\n  - openapi/workday-benefits-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/authentication/workday-benefits-authentication.yml
summary_line: oauth2 · 1 scheme
tags: []
---
