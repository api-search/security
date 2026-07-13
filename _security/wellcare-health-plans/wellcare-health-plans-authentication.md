---
api_key_in: []
api_specs:
- filename: wellcare-fhir-patient-access-api-openapi.yml
  format: yaml
  label: WellCare FHIR Patient Access API
  slug: fhir-patient-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-fhir-patient-access-api-openapi.yml
- filename: wellcare-fhir-provider-directory-api-openapi.yml
  format: yaml
  label: WellCare FHIR Provider Directory API
  slug: fhir-provider-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-fhir-provider-directory-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Wellcare Health Plans Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: wellcare-health-plans secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: wellcare-health-plans
provider_slug: wellcare-health-plans
scheme_count: 2
schemes:
- description: SMART on FHIR OAuth 2.0 authorization for patient-facing apps.
  flows:
  - authorizationUrl: https://partners.centene.com/oauth2/authorize
    flow: authorizationCode
    scopes: 8
    tokenUrl: https://partners.centene.com/oauth2/token
  name: smartOnFhir
  sources:
  - openapi/wellcare-fhir-patient-access-api-openapi.yml
  type: oauth2
- description: Bearer token from Centene Partner Portal OAuth 2.0 authorization.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/wellcare-fhir-provider-directory-api-openapi.yml
  type: http
slug: wellcare-health-plans-authentication
source_filename: wellcare-health-plans-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wellcare-fhir-patient-access-api-openapi.yml, openapi/wellcare-fhir-provider-directory-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: smartOnFhir\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://partners.centene.com/oauth2/authorize\n    tokenUrl: https://partners.centene.com/oauth2/token\n    scopes: 8\n  description: SMART on FHIR OAuth 2.0 authorization for patient-facing apps.\n  sources:\n  - openapi/wellcare-fhir-patient-access-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token from Centene Partner Portal OAuth 2.0 authorization.\n  sources:\n  - openapi/wellcare-fhir-provider-directory-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/authentication/wellcare-health-plans-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Fortune 500
---
