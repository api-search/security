---
api_key_in: []
api_specs:
- filename: cerner-oracle-health-fhir-r4-api-openapi.yml
  format: yaml
  label: Oracle Health Millennium Platform FHIR R4 API
  slug: oracle-health-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/openapi/cerner-oracle-health-fhir-r4-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cerner Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Cerner (Oracle Health) secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Cerner (Oracle Health)
provider_slug: cerner
scheme_count: 1
schemes:
- description: SMART on FHIR OAuth 2.0 with patient, user, and system scopes.
  flows:
  - authorizationUrl: https://authorization.cerner.com/tenants/{tenant}/protocols/oauth2/profiles/smart-v1/personas/patient/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://authorization.cerner.com/tenants/{tenant}/protocols/oauth2/profiles/smart-v1/token
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://authorization.cerner.com/tenants/{tenant}/protocols/oauth2/profiles/smart-v1/token
  name: oauth2
  sources:
  - openapi/cerner-oracle-health-fhir-r4-api-openapi.yml
  type: oauth2
slug: cerner-authentication
source_filename: cerner-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cerner-oracle-health-fhir-r4-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authorization.cerner.com/tenants/{tenant}/protocols/oauth2/profiles/smart-v1/personas/patient/authorize\n    tokenUrl: https://authorization.cerner.com/tenants/{tenant}/protocols/oauth2/profiles/smart-v1/token\n    scopes: 3\n  - flow: clientCredentials\n    tokenUrl: https://authorization.cerner.com/tenants/{tenant}/protocols/oauth2/profiles/smart-v1/token\n    scopes: 2\n  description: SMART on FHIR OAuth 2.0 with patient, user, and system scopes.\n  sources:\n  - openapi/cerner-oracle-health-fhir-r4-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/authentication/cerner-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Cerner Millennium
- Code Console
- EHR
- Electronic Health Records
- FHIR
- HL7
- Healthcare
- Interoperability
- OAuth 2.0
- Oracle Health
- Patient Access
- Provider Directory
- SMART on FHIR
- Fortune 1000
---
