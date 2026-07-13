---
api_key_in: []
api_specs:
- filename: athenahealth-athenaone-rest-api-openapi.yml
  format: yaml
  label: athenahealth athenaOne REST API
  slug: athenahealth-athenaone-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/openapi/athenahealth-athenaone-rest-api-openapi.yml
- filename: athenahealth-fhir-r4-api-openapi.yml
  format: yaml
  label: athenahealth FHIR R4 API
  slug: athenahealth-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/openapi/athenahealth-fhir-r4-api-openapi.yml
- filename: athenahealth-fhir-subscriptions-api-openapi.yml
  format: yaml
  label: athenahealth FHIR Subscriptions API
  slug: athenahealth-fhir-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/openapi/athenahealth-fhir-subscriptions-api-openapi.yml
- filename: athenahealth-fhir-bulk-data-api-openapi.yml
  format: yaml
  label: athenahealth FHIR Bulk Data Access API
  slug: athenahealth-fhir-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/openapi/athenahealth-fhir-bulk-data-api-openapi.yml
- filename: athenahealth-cds-hooks-api-openapi.yml
  format: yaml
  label: athenahealth CDS Hooks API
  slug: athenahealth-cds-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/openapi/athenahealth-cds-hooks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Athena Health Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: athenahealth secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: athenahealth
provider_slug: athena-health
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.platform.athenahealth.com/oauth2/v1/token
  - authorizationUrl: https://api.platform.athenahealth.com/oauth2/v1/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.platform.athenahealth.com/oauth2/v1/token
  name: oauth2
  sources:
  - openapi/athenahealth-athenaone-rest-api-openapi.yml
  - openapi/athenahealth-fhir-r4-api-openapi.yml
  type: oauth2
- description: SMART Backend Services (JWT client assertion)
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.platform.athenahealth.com/oauth2/v1/token
  name: backend
  sources:
  - openapi/athenahealth-fhir-bulk-data-api-openapi.yml
  - openapi/athenahealth-fhir-subscriptions-api-openapi.yml
  type: oauth2
slug: athena-health-authentication
source_filename: athena-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/athenahealth-athenaone-rest-api-openapi.yml, openapi/athenahealth-fhir-bulk-data-api-openapi.yml,\n  openapi/athenahealth-fhir-r4-api-openapi.yml, openapi/athenahealth-fhir-subscriptions-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.platform.athenahealth.com/oauth2/v1/token\n    scopes: 1\n  - flow: authorizationCode\n    authorizationUrl: https://api.platform.athenahealth.com/oauth2/v1/authorize\n    tokenUrl: https://api.platform.athenahealth.com/oauth2/v1/token\n    scopes: 1\n  sources:\n  - openapi/athenahealth-athenaone-rest-api-openapi.yml\n  - openapi/athenahealth-fhir-r4-api-openapi.yml\n- name: backend\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.platform.athenahealth.com/oauth2/v1/token\n    scopes:\
  \ 1\n  description: SMART Backend Services (JWT client assertion)\n  sources:\n  - openapi/athenahealth-fhir-bulk-data-api-openapi.yml\n  - openapi/athenahealth-fhir-subscriptions-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/authentication/athena-health-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- EHR
- Electronic Health Records
- Healthcare
- HL7
- FHIR
- Interoperability
- Practice Management
- Revenue Cycle Management
- USCDI
- Cures Act
- SMART on FHIR
- CDS Hooks
- Cloud EHR
---
