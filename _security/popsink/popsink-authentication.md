---
api_key_in: []
api_specs:
- filename: popsink-public-api-openapi-original.json
  format: json
  label: Popsink Public API
  slug: popsink-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popsink/refs/heads/main/openapi/popsink-public-api-openapi-original.json
- filename: popsink-onprem-api-openapi-original.json
  format: json
  label: Popsink Control Plane API
  slug: popsink-control-plane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popsink/refs/heads/main/openapi/popsink-onprem-api-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Popsink Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Popsink secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Popsink
provider_slug: popsink
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 0
    tokenUrl: auth/jwt/login
  name: OAuth2PasswordBearer
  sources:
  - openapi/popsink-onprem-api-openapi-original.json
  type: oauth2
slug: popsink-authentication
source_filename: popsink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/popsink-onprem-api-openapi-original.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: OAuth2PasswordBearer\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: auth/jwt/login\n    scopes: 0\n  sources:\n  - openapi/popsink-onprem-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/popsink/refs/heads/main/authentication/popsink-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Change Data Capture
- Data Replication
- CDC
- Data Integration
- Real-Time Data
- Streaming
- ETL
- Database
- Data Platform
---
