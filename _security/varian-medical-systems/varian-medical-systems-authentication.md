---
api_key_in: []
api_specs:
- filename: varian-medical-systems-allergyintolerance-api-openapi.yml
  format: yaml
  label: Varian Medical Systems AllergyIntolerance API
  slug: varian-medical-systems-allergyintolerance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-allergyintolerance-api-openapi.yml
- filename: varian-medical-systems-careplan-api-openapi.yml
  format: yaml
  label: Varian Medical Systems CarePlan API
  slug: varian-medical-systems-careplan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-careplan-api-openapi.yml
- filename: varian-medical-systems-condition-api-openapi.yml
  format: yaml
  label: Varian Medical Systems Condition API
  slug: varian-medical-systems-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-condition-api-openapi.yml
- filename: varian-medical-systems-diagnosticreport-api-openapi.yml
  format: yaml
  label: Varian Medical Systems DiagnosticReport API
  slug: varian-medical-systems-diagnosticreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-diagnosticreport-api-openapi.yml
- filename: varian-medical-systems-documentreference-api-openapi.yml
  format: yaml
  label: Varian Medical Systems DocumentReference API
  slug: varian-medical-systems-documentreference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-documentreference-api-openapi.yml
- filename: varian-medical-systems-goal-api-openapi.yml
  format: yaml
  label: Varian Medical Systems Goal API
  slug: varian-medical-systems-goal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-goal-api-openapi.yml
- filename: varian-medical-systems-medicationrequest-api-openapi.yml
  format: yaml
  label: Varian Medical Systems MedicationRequest API
  slug: varian-medical-systems-medicationrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-medicationrequest-api-openapi.yml
- filename: varian-medical-systems-metadata-api-openapi.yml
  format: yaml
  label: Varian Medical Systems Metadata API
  slug: varian-medical-systems-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-metadata-api-openapi.yml
- filename: varian-medical-systems-observation-api-openapi.yml
  format: yaml
  label: Varian Medical Systems Observation API
  slug: varian-medical-systems-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-observation-api-openapi.yml
- filename: varian-medical-systems-patient-api-openapi.yml
  format: yaml
  label: Varian Medical Systems Patient API
  slug: varian-medical-systems-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-patient-api-openapi.yml
- filename: varian-medical-systems-procedure-api-openapi.yml
  format: yaml
  label: Varian Medical Systems Procedure API
  slug: varian-medical-systems-procedure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-procedure-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Varian Medical Systems Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Varian Medical Systems secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Varian Medical Systems
provider_slug: varian-medical-systems
scheme_count: 1
schemes:
- description: SMART on FHIR OAuth 2.0 authorization
  flows:
  - authorizationUrl: https://varian-smart.dynamicfhir.com/core/connect/authorize
    flow: authorizationCode
    scopes: 11
    tokenUrl: https://varian-smart.dynamicfhir.com/core/connect/token
  name: OAuthSMARTonFHIR
  sources:
  - openapi/varian-aria-fhir-openapi.yml
  type: oauth2
slug: varian-medical-systems-authentication
source_filename: varian-medical-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/varian-aria-fhir-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuthSMARTonFHIR\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://varian-smart.dynamicfhir.com/core/connect/authorize\n    tokenUrl: https://varian-smart.dynamicfhir.com/core/connect/token\n    scopes: 11\n  description: SMART on FHIR OAuth 2.0 authorization\n  sources:\n  - openapi/varian-aria-fhir-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/authentication/varian-medical-systems-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Healthcare
- Oncology
- Medical Devices
- FHIR
- Radiation Therapy
- Health IT
- Fortune 1000
---
