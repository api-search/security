---
api_key_in: []
api_specs:
- filename: llms.txt
  format: yaml
  label: Elation Health REST API
  slug: elation-health-api
  spec_type: OpenAPI
  url: https://docs.elationhealth.com/llms.txt
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Elation Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Elation Health secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Elation Health
provider_slug: elation
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://sandbox.elationemr.com/api/2.0/oauth2/token/
  name: oauth2
  sources:
  - openapi/elation-elation-health-api-openapi.yml
  type: oauth2
slug: elation-authentication
source_filename: elation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/elation-elation-health-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.elationemr.com/api/2.0/oauth2/token/\n    scopes: 1\n  sources:\n  - openapi/elation-elation-health-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/authentication/elation-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- EHR
- Electronic Health Records
- Primary Care
- Healthcare
- FHIR
- Clinical
- Patients
- Prescriptions
- Messaging
---
