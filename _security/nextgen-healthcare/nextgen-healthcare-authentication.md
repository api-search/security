---
api_key_in: []
api_specs:
- filename: nextgen-office-fhir-r4-openapi.yaml
  format: yaml
  label: NextGen Office FHIR R4 API
  slug: nextgen-office-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextgen-healthcare/refs/heads/main/openapi/nextgen-office-fhir-r4-openapi.yaml
- filename: nextgen-office-bulk-fhir-r4-openapi.yml
  format: yaml
  label: NextGen Office Bulk FHIR R4 API
  slug: nextgen-office-bulk-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextgen-healthcare/refs/heads/main/openapi/nextgen-office-bulk-fhir-r4-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Nextgen Healthcare Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: NextGen Healthcare secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: NextGen Healthcare
provider_slug: nextgen-healthcare
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nextgen-office-bulk-fhir-r4-openapi.yml
  type: http
- description: Access code based oauth authentication
  flows:
  - authorizationUrl: https://idp-prod.prod.ngo.nextgenaws.net/auth/realms/nextgen/protocol/openid-connect/auth?aud=https://fhir.meditouchehr.com/api/fhir/r4
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://idp-prod.prod.ngo.nextgenaws.net/auth/realms/nextgen/protocol/openid-connect/token
  name: OauthSecurity
  sources:
  - openapi/nextgen-office-fhir-r4-openapi.yaml
  type: oauth2
slug: nextgen-healthcare-authentication
source_filename: nextgen-healthcare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: derived\nsource: openapi/nextgen-office-bulk-fhir-r4-openapi.yml, openapi/nextgen-office-fhir-r4-openapi.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/nextgen-office-bulk-fhir-r4-openapi.yml\n- name: OauthSecurity\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://idp-prod.prod.ngo.nextgenaws.net/auth/realms/nextgen/protocol/openid-connect/auth?aud=https://fhir.meditouchehr.com/api/fhir/r4\n    tokenUrl: https://idp-prod.prod.ngo.nextgenaws.net/auth/realms/nextgen/protocol/openid-connect/token\n    scopes: 4\n  description: Access code based oauth authentication\n  sources:\n  - openapi/nextgen-office-fhir-r4-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextgen-healthcare/refs/heads/main/authentication/nextgen-healthcare-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Healthcare
- United States
- EHR
- EMR
- FHIR
- HL7
- Interoperability
- SMART on FHIR
- USCDI
- Bulk FHIR
- Patient Access
- 21st Century Cures
---
