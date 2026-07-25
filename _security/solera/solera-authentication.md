---
api_key_in:
- header
api_specs:
- filename: solera-dashboard-assignment-openapi.json
  format: json
  label: Solera Dashboard Assignment API
  slug: solera-dashboard-assignment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-dashboard-assignment-openapi.json
- filename: solera-claim-images-openapi.json
  format: json
  label: Solera ClaimImages API
  slug: solera-claim-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-claim-images-openapi.json
- filename: solera-gic-integration-openapi.json
  format: json
  label: Solera EAPI GIC Integration API
  slug: solera-gic-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-gic-integration-openapi.json
- filename: solera-getdocuments-v1-openapi.json
  format: json
  label: Audatex GetDocuments API
  slug: solera-getdocuments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-getdocuments-v1-openapi.json
- filename: solera-getimage-v1-openapi.json
  format: json
  label: Audatex Assignment Get Document API (GetImage)
  slug: solera-getimage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-getimage-v1-openapi.json
- filename: solera-eapi-getdocument-openapi.json
  format: json
  label: Solera EAPI Get Document API
  slug: solera-eapi-getdocument-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-eapi-getdocument-openapi.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Solera Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Solera secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Solera
provider_slug: solera
scheme_count: 2
schemes:
- description: Authorization using the JWT Bearer scheme
  flows:
  - flow: password
    scopes: 1
    tokenUrl: https://dispatch-login-demo.audatex.com/connect/token
  name: oauth2
  sources:
  - openapi/solera-claim-images-openapi.json
  - openapi/solera-claim-images-prod-swagger.json
  - openapi/solera-dashboard-assignment-openapi.json
  - openapi/solera-eapi-getdocument-openapi.json
  - openapi/solera-enterprise-assignment-prod-swagger.json
  - openapi/solera-getdocuments-v1-openapi.json
  - openapi/solera-getdocuments-v2-openapi.json
  - openapi/solera-gic-integration-openapi.json
  type: oauth2
- description: Authorization header using the Bearer scheme
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/solera-getimage-v1-openapi.json
  - openapi/solera-getimage-v2-openapi.json
  type: apiKey
slug: solera-authentication
source_filename: solera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: derived\nsource: openapi/solera-claim-images-openapi.json, openapi/solera-claim-images-prod-swagger.json,\n  openapi/solera-dashboard-assignment-openapi.json, openapi/solera-eapi-getdocument-openapi.json,\n  openapi/solera-enterprise-assignment-prod-swagger.json, openapi/solera-getdocuments-v1-openapi.json,\n  openapi/solera-getdocuments-v2-openapi.json, openapi/solera-getimage-v1-openapi.json, openapi/solera-getimage-v2-openapi.json,\n  openapi/solera-gic-integration-openapi.json\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - password\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://dispatch-login-demo.audatex.com/connect/token\n    scopes: 1\n  description: Authorization using the JWT Bearer scheme\n  sources:\n  - openapi/solera-claim-images-openapi.json\n  - openapi/solera-claim-images-prod-swagger.json\n  - openapi/solera-dashboard-assignment-openapi.json\n\
  \  - openapi/solera-eapi-getdocument-openapi.json\n  - openapi/solera-enterprise-assignment-prod-swagger.json\n  - openapi/solera-getdocuments-v1-openapi.json\n  - openapi/solera-getdocuments-v2-openapi.json\n  - openapi/solera-gic-integration-openapi.json\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Authorization header using the Bearer scheme\n  sources:\n  - openapi/solera-getimage-v1-openapi.json\n  - openapi/solera-getimage-v2-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/authentication/solera-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Insurance
- United States
- Property and Casualty
- Claims
- Claims Technology
- Automotive Claims
- FNOL
- Vehicle Damage Assessment
- Risk Data
- CIECA
- Insurtech
---
