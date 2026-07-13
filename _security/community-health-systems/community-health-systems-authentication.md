---
api_key_in: []
api_specs:
- filename: chs-patient-access-api-openapi.yml
  format: yaml
  label: Community Health Systems Patient Access API
  slug: patient-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/community-health-systems/refs/heads/main/openapi/chs-patient-access-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Community Health Systems Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Community Health Systems secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Community Health Systems
provider_slug: community-health-systems
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://api.chs.net/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.chs.net/oauth2/token
  name: oauth2
  sources:
  - openapi/chs-patient-access-api-openapi.yml
  type: oauth2
slug: community-health-systems-authentication
source_filename: community-health-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chs-patient-access-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.chs.net/oauth2/authorize\n    tokenUrl: https://api.chs.net/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/chs-patient-access-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/community-health-systems/refs/heads/main/authentication/community-health-systems-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- CMS-9115-F
- FHIR
- Healthcare
- Hospitals
- Interoperability
- Patient Access
- Provider Directory
- SMART-on-FHIR
- Fortune 500
---
