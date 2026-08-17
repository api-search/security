---
api_key_in:
- header
api_specs:
- filename: tebra-documents-api-openapi.yml
  format: yaml
  label: Tebra Documents API
  slug: tebra-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tebra/refs/heads/main/openapi/tebra-documents-api-openapi.yml
- filename: tebra-clinical-api-openapi.yml
  format: yaml
  label: Tebra Clinical API
  slug: tebra-clinical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tebra/refs/heads/main/openapi/tebra-clinical-api-openapi.yml
- filename: tebra-documents-api-openapi.yml
  format: yaml
  label: Tebra Documents API
  slug: tebra-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tebra/refs/heads/main/openapi/tebra-documents-api-openapi.yml
- filename: tebra-patient-api-openapi.yml
  format: yaml
  label: Tebra Patient API
  slug: tebra-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tebra/refs/heads/main/openapi/tebra-patient-api-openapi.yml
- filename: tebra-fhir-api-openapi.yml
  format: yaml
  label: Tebra FHIR API
  slug: tebra-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tebra/refs/heads/main/openapi/tebra-fhir-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Tebra Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Tebra secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Tebra
provider_slug: tebra
scheme_count: 3
schemes:
- description: Patient-generated API Key from the Tebra Patient Portal (My Account > API Access Key). A missing, revoked, or invalid key returns 401 Unauthorized.
  in: header
  name: apiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/tebra-clinical-api-openapi.yml
  - openapi/tebra-documents-api-openapi.yml
  - openapi/tebra-patient-api-openapi.yml
  type: apiKey
- description: SMART on FHIR 3-legged OAuth 2.0 authorization-code flow for user-facing (patient/provider) applications. Authorization/token URLs are confirmed verbatim from the Tebra FHIR API User Guide. The scope list below is DERIVED, not verbatim - Tebra's guide instructs developers to "enter the SMART scopes required" without publishing an enumerated list, so these are the standard SMART v1 `patient/<Resour
  flows:
  - authorizationUrl: https://fhir.prd.cloud.tebra.com/smartauth/oauth/authorize
    flow: authorizationCode
    scopes: 24
    tokenUrl: https://fhir.prd.cloud.tebra.com/smartauth/oauth/token
  name: smartOnFhirAuthCode
  sources:
  - openapi/tebra-fhir-api-openapi.yml
  type: oauth2
- description: SMART on FHIR 2-legged OAuth 2.0 client-credentials flow for backend services applications (no end-user present). Token endpoint is confirmed verbatim from the Tebra FHIR API User Guide; Tebra currently supports only the Client Credentials workflow (not JWKS-based backend auth). Scope strings below are DERIVED (`system/<Resource>.read`, standard SMART v1 syntax), not verbatim - see note above.
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://fhir.prd.cloud.tebra.com/smartauth/oauth/token
  name: smartOnFhirClientCredentials
  sources:
  - openapi/tebra-fhir-api-openapi.yml
  type: oauth2
slug: tebra-authentication
source_filename: tebra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/tebra-clinical-api-openapi.yml, openapi/tebra-documents-api-openapi.yml, openapi/tebra-fhir-api-openapi.yml,\n  openapi/tebra-patient-api-openapi.yml\ndocs:\n- https://www.tebra.com/wp-content/uploads/2025/05/Tebra-FHIR-API-User-Guide.pdf\n- https://www.tebra.com/wp-content/uploads/2023/10/General_API_Documentation-Tebra.pdf\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Patient-generated API Key from the Tebra Patient Portal (My Account > API Access\n    Key). A missing, revoked, or invalid key returns 401 Unauthorized.\n  sources:\n  - openapi/tebra-clinical-api-openapi.yml\n  - openapi/tebra-documents-api-openapi.yml\n  - openapi/tebra-patient-api-openapi.yml\n- name: smartOnFhirAuthCode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://fhir.prd.cloud.tebra.com/smartauth/oauth/authorize\n    tokenUrl: https://fhir.prd.cloud.tebra.com/smartauth/oauth/token\n    scopes: 24\n  description: SMART on FHIR 3-legged OAuth 2.0 authorization-code flow for user-facing (patient/provider)\n    applications. Authorization/token URLs are confirmed verbatim from the Tebra FHIR API User\n    Guide. The scope list below is DERIVED, not verbatim - Tebra's guide instructs developers\n    to \"enter the SMART scopes required\" without publishing an enumerated list, so these are\n    the standard SMART v1 `patient/<Resour\n  sources:\n  - openapi/tebra-fhir-api-openapi.yml\n- name: smartOnFhirClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://fhir.prd.cloud.tebra.com/smartauth/oauth/token\n    scopes: 3\n  description: SMART on FHIR 2-legged OAuth 2.0 client-credentials flow for backend services\n    applications (no end-user present). Token endpoint is confirmed\
  \ verbatim from the Tebra\n    FHIR API User Guide; Tebra currently supports only the Client Credentials workflow (not\n    JWKS-based backend auth). Scope strings below are DERIVED (`system/<Resource>.read`, standard\n    SMART v1 syntax), not verbatim - see note above.\n  sources:\n  - openapi/tebra-fhir-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tebra/refs/heads/main/authentication/tebra-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Healthcare
- Practice Management
- EHR
- Medical Billing
- Patient Engagement
- Kareo
- PatientPop
---
