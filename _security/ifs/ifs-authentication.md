---
api_key_in: []
api_specs:
- filename: ifs-finance-api-openapi.yml
  format: yaml
  label: IFS Finance API
  slug: ifs-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ifs/refs/heads/main/openapi/ifs-finance-api-openapi.yml
- filename: ifs-inventory-api-openapi.yml
  format: yaml
  label: IFS Inventory API
  slug: ifs-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ifs/refs/heads/main/openapi/ifs-inventory-api-openapi.yml
- filename: ifs-procurement-api-openapi.yml
  format: yaml
  label: IFS Procurement API
  slug: ifs-procurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ifs/refs/heads/main/openapi/ifs-procurement-api-openapi.yml
- filename: ifs-work-orders-api-openapi.yml
  format: yaml
  label: IFS Work Orders API
  slug: ifs-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ifs/refs/heads/main/openapi/ifs-work-orders-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ifs Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: IFS secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: IFS
provider_slug: ifs
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://login.ifs.cloud/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://login.ifs.cloud/oauth2/token
  name: OAuth2
  sources:
  - openapi/ifs-cloud-erp-openapi.yml
  type: oauth2
slug: ifs-authentication
source_filename: ifs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ifs-cloud-erp-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.ifs.cloud/oauth2/authorize\n    tokenUrl: https://login.ifs.cloud/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/ifs-cloud-erp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ifs/refs/heads/main/authentication/ifs-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- ERP
- Field Service
- Asset Management
- Manufacturing
- Energy
- Cloud
- Sweden
---
