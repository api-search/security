---
api_key_in: []
api_specs:
- filename: independence-blue-cross-formulary-api-openapi.yml
  format: yaml
  label: Independence Blue Cross Formulary API
  slug: independence-blue-cross-formulary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/independence-blue-cross/refs/heads/main/openapi/independence-blue-cross-formulary-api-openapi.yml
- filename: independence-blue-cross-patient-access-api-openapi.yml
  format: yaml
  label: Independence Blue Cross Patient Access API
  slug: independence-blue-cross-patient-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/independence-blue-cross/refs/heads/main/openapi/independence-blue-cross-patient-access-api-openapi.yml
- filename: independence-blue-cross-provider-directory-api-openapi.yml
  format: yaml
  label: Independence Blue Cross Provider Directory API
  slug: independence-blue-cross-provider-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/independence-blue-cross/refs/heads/main/openapi/independence-blue-cross-provider-directory-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Independence Blue Cross Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Independence Blue Cross secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Independence Blue Cross
provider_slug: independence-blue-cross
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://member.ibx.com/patientaccesssvc/oauth2/v1/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://eapics.ibx.com/oauth2/v2/token
  name: smart_on_fhir
  sources:
  - openapi/independence-blue-cross-patient-openapi.yml
  type: oauth2
slug: independence-blue-cross-authentication
source_filename: independence-blue-cross-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/independence-blue-cross-patient-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: smart_on_fhir\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://member.ibx.com/patientaccesssvc/oauth2/v1/authorize\n    tokenUrl: https://eapics.ibx.com/oauth2/v2/token\n    scopes: 4\n  sources:\n  - openapi/independence-blue-cross-patient-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/independence-blue-cross/refs/heads/main/authentication/independence-blue-cross-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Healthcare
- Health Insurance
- Blue Cross Blue Shield
- Managed Care
- Medicare
- Medicare Advantage
- Medicaid
- CHIP
- Commercial
- Dental
- Vision
- Behavioral Health
- Pharmacy Benefits
- Interoperability
- FHIR
- SMART On FHIR
- CMS
- Patient Access
- Provider Directory
- Drug Formulary
- Transparency In Coverage
---
