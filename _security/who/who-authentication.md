---
api_key_in: []
api_specs:
- filename: $metadata
  format: yaml
  label: WHO GHO OData API
  slug: who-gho-odata-api
  spec_type: OpenAPI
  url: https://ghoapi.azureedge.net/api/$metadata
- filename: index.html
  format: yaml
  label: WHO ICD API
  slug: who-icd-api
  spec_type: OpenAPI
  url: https://id.who.int/swagger/index.html
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Who Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: World Health Organization (WHO) secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: World Health Organization (WHO)
provider_slug: who
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://icdaccessmanagement.who.int/connect/token
  name: oauth2
  sources:
  - openapi/who-icd-api-openapi.json
  type: oauth2
slug: who-authentication
source_filename: who-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/who-icd-api-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://icdaccessmanagement.who.int/connect/token\n    scopes: 1\n  sources:\n  - openapi/who-icd-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/who/refs/heads/main/authentication/who-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Health
- Global Health
- Disease Surveillance
- Immunization
- Health Statistics
- ICD
- WHO
- United Nations
- Open Data
---
