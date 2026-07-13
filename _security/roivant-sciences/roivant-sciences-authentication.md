---
api_key_in: []
api_specs:
- filename: datavant-healthjump-ehr-openapi.yml
  format: yaml
  label: Datavant Healthjump EHR Integration API
  slug: datavant-healthjump-ehr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/datavant-healthjump-ehr-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Roivant Sciences Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Roivant Sciences secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Roivant Sciences
provider_slug: roivant-sciences
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://api.healthjump.com/oauth/token
  name: OAuth2
  sources:
  - openapi/datavant-healthjump-ehr-openapi.yml
  type: oauth2
slug: roivant-sciences-authentication
source_filename: roivant-sciences-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/datavant-healthjump-ehr-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.healthjump.com/oauth/token\n    scopes: 3\n  sources:\n  - openapi/datavant-healthjump-ehr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/authentication/roivant-sciences-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Biotech
- Pharmaceutical
- Drug Development
- Clinical Trials
- Health Data
- Tokenization
- Electronic Health Records
- Real World Evidence
- Holding Company
- Healthcare
---
