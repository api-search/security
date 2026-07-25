---
api_key_in: []
api_specs:
- filename: drchrono-administrative-api-openapi.yml
  format: yaml
  label: drchrono Administrative API
  slug: drchrono-administrative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-administrative-api-openapi.yml
- filename: drchrono-audit-api-openapi.yml
  format: yaml
  label: drchrono Audit API
  slug: drchrono-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-audit-api-openapi.yml
- filename: drchrono-availability-api-openapi.yml
  format: yaml
  label: drchrono Availability API
  slug: drchrono-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-availability-api-openapi.yml
- filename: drchrono-billing-api-openapi.yml
  format: yaml
  label: drchrono Billing API
  slug: drchrono-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-billing-api-openapi.yml
- filename: drchrono-clinical-api-openapi.yml
  format: yaml
  label: drchrono Clinical API
  slug: drchrono-clinical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-clinical-api-openapi.yml
- filename: drchrono-practice-management-api-openapi.yml
  format: yaml
  label: drchrono Practice Management API
  slug: drchrono-practice-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-practice-management-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Drchrono Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: drchrono secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: drchrono
provider_slug: drchrono
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://app.drchrono.com/o/authorize/
    flow: authorizationCode
    scopes: 22
    tokenUrl: https://app.drchrono.com/o/token/
  name: drchrono_oauth2
  sources:
  - openapi/drchrono-rest-api-openapi.yml
  type: oauth2
slug: drchrono-authentication
source_filename: drchrono-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/drchrono-rest-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: drchrono_oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.drchrono.com/o/authorize/\n    tokenUrl: https://app.drchrono.com/o/token/\n    scopes: 22\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/authentication/drchrono-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- EHR
- Electronic Health Records
- Healthcare
- Medical Records
- Practice Management
- HIPAA
- Appointments
- Billing
- Prescriptions
- Lab Integration
- FHIR
---
