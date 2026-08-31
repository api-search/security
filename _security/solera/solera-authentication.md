---
api_key_in:
- header
api_specs:
- filename: solera-assignment-api-openapi.yml
  format: yaml
  label: Solera Assignment API
  slug: solera-assignment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-assignment-api-openapi.yml
- filename: solera-estimatereturn-api-openapi.yml
  format: yaml
  label: Solera Estimate Return API
  slug: solera-estimatereturn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-estimatereturn-api-openapi.yml
- filename: solera-getclaimimageresponse-api-openapi.yml
  format: yaml
  label: Solera Get Claim Image Response API
  slug: solera-getclaimimageresponse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-getclaimimageresponse-api-openapi.yml
- filename: solera-getdocument-api-openapi.yml
  format: yaml
  label: Solera Get Document API
  slug: solera-getdocument-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-getdocument-api-openapi.yml
- filename: solera-getdocuments-api-openapi.yml
  format: yaml
  label: Solera Get Documents API
  slug: solera-getdocuments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-getdocuments-api-openapi.yml
- filename: solera-getimage-api-openapi.yml
  format: yaml
  label: Solera Get Image API
  slug: solera-getimage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-getimage-api-openapi.yml
- filename: solera-getvaluation-api-openapi.yml
  format: yaml
  label: Solera Get Valuation API
  slug: solera-getvaluation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-getvaluation-api-openapi.yml
- filename: solera-getvaluationresponse-api-openapi.yml
  format: yaml
  label: Solera Get Valuation Response API
  slug: solera-getvaluationresponse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-getvaluationresponse-api-openapi.yml
- filename: solera-gicintegration-api-openapi.yml
  format: yaml
  label: Solera GIC Integration API
  slug: solera-gicintegration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-gicintegration-api-openapi.yml
- filename: solera-valuationreturn-api-openapi.yml
  format: yaml
  label: Solera Valuation Return API
  slug: solera-valuationreturn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-valuationreturn-api-openapi.yml
- filename: solera-version-api-openapi.yml
  format: yaml
  label: Solera Version API
  slug: solera-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-version-api-openapi.yml
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
