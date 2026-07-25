---
api_key_in: []
api_specs:
- filename: pointclickcare-assessments-api-openapi.yml
  format: yaml
  label: PointClickCare Assessments API
  slug: pointclickcare-assessments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pointclickcare/refs/heads/main/openapi/pointclickcare-assessments-api-openapi.yml
- filename: pointclickcare-diagnoses-api-openapi.yml
  format: yaml
  label: PointClickCare Diagnoses API
  slug: pointclickcare-diagnoses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pointclickcare/refs/heads/main/openapi/pointclickcare-diagnoses-api-openapi.yml
- filename: pointclickcare-facilities-api-openapi.yml
  format: yaml
  label: PointClickCare Facilities API
  slug: pointclickcare-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pointclickcare/refs/heads/main/openapi/pointclickcare-facilities-api-openapi.yml
- filename: pointclickcare-medications-api-openapi.yml
  format: yaml
  label: PointClickCare Medications API
  slug: pointclickcare-medications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pointclickcare/refs/heads/main/openapi/pointclickcare-medications-api-openapi.yml
- filename: pointclickcare-patients-api-openapi.yml
  format: yaml
  label: PointClickCare Patients API
  slug: pointclickcare-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pointclickcare/refs/heads/main/openapi/pointclickcare-patients-api-openapi.yml
- filename: pointclickcare-vitals-api-openapi.yml
  format: yaml
  label: PointClickCare Vitals API
  slug: pointclickcare-vitals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pointclickcare/refs/heads/main/openapi/pointclickcare-vitals-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Pointclickcare Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: PointClickCare secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: PointClickCare
provider_slug: pointclickcare
scheme_count: 1
schemes:
- description: OAuth2 authorization code flow via PointClickCare identity server
  flows:
  - authorizationUrl: https://login.pointclickcare.com/oauth2/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://login.pointclickcare.com/oauth2/token
  name: oauth2
  sources:
  - openapi/pointclickcare-ehr-openapi.yml
  type: oauth2
slug: pointclickcare-authentication
source_filename: pointclickcare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pointclickcare-ehr-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.pointclickcare.com/oauth2/authorize\n    tokenUrl: https://login.pointclickcare.com/oauth2/token\n    scopes: 3\n  description: OAuth2 authorization code flow via PointClickCare identity server\n  sources:\n  - openapi/pointclickcare-ehr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pointclickcare/refs/heads/main/authentication/pointclickcare-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Healthcare
- Long-Term Care
- Post-Acute Care
- EHR
- FHIR
- Senior Care
- Interoperability
---
