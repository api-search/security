---
api_key_in: []
api_specs:
- filename: tenet-healthcare-fhir-openapi.yml
  format: yaml
  label: Tenet Health Patient Portal API
  slug: tenet-health-patient-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenet-healthcare/refs/heads/main/openapi/tenet-healthcare-fhir-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Tenet Healthcare Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Tenet Healthcare secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Tenet Healthcare
provider_slug: tenet-healthcare
scheme_count: 1
schemes:
- description: SMART on FHIR OAuth 2.0 authorization
  flows:
  - authorizationUrl: https://auth.tenethealth.com/oauth2/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://auth.tenethealth.com/oauth2/token
  name: smartOnFhir
  sources:
  - openapi/tenet-healthcare-fhir-openapi.yml
  type: oauth2
slug: tenet-healthcare-authentication
source_filename: tenet-healthcare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tenet-healthcare-fhir-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: smartOnFhir\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.tenethealth.com/oauth2/authorize\n    tokenUrl: https://auth.tenethealth.com/oauth2/token\n    scopes: 6\n  description: SMART on FHIR OAuth 2.0 authorization\n  sources:\n  - openapi/tenet-healthcare-fhir-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tenet-healthcare/refs/heads/main/authentication/tenet-healthcare-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Healthcare
- Hospitals
- Ambulatory Surgery Centers
- Revenue Cycle Management
- Fortune 500
---
