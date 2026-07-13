---
api_key_in: []
api_specs:
- filename: sas-viya-rest-api-openapi.yml
  format: yaml
  label: SAS Viya REST API
  slug: viya-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-viya-rest-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sas Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: SAS Institute secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: SAS Institute
provider_slug: sas
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 1
    tokenUrl: /SASLogon/oauth/token
  name: oauth2
  sources:
  - openapi/sas-viya-rest-api-openapi.yml
  type: oauth2
slug: sas-authentication
source_filename: sas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sas-viya-rest-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: /SASLogon/oauth/token\n    scopes: 1\n  sources:\n  - openapi/sas-viya-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/authentication/sas-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Analytics
- Data Management
- Artificial Intelligence
- Machine Learning
- Software
---
