---
api_key_in: []
api_specs:
- filename: smarthealthit-openapi.yml
  format: yaml
  label: SMART Sandbox FHIR R4 API
  slug: smarthealthit-sandbox-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthealthit/refs/heads/main/openapi/smarthealthit-openapi.yml
- filename: smarthealthit-openapi.yml
  format: yaml
  label: SMART App Launch Authorization API
  slug: smarthealthit-smart-app-launch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthealthit/refs/heads/main/openapi/smarthealthit-openapi.yml
- filename: smarthealthit-openapi.yml
  format: yaml
  label: SMART Bulk Data Export API
  slug: smarthealthit-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthealthit/refs/heads/main/openapi/smarthealthit-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Smarthealthit Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: SMART Health IT secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: SMART Health IT
provider_slug: smarthealthit
scheme_count: 1
schemes:
- description: HL7 SMART App Launch OAuth 2.0 profile, used by the launcher's protected FHIR proxy. The open r4.smarthealthit.org sandbox requires no authentication; the Bulk Data server uses SMART Backend Services (client_credentials with a signed JWT assertion).
  flows:
  - authorizationUrl: https://launch.smarthealthit.org/v/r4/auth/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://launch.smarthealthit.org/v/r4/auth/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://launch.smarthealthit.org/v/r4/auth/token
  name: smartOnFhir
  sources:
  - openapi/smarthealthit-openapi.yml
  type: oauth2
slug: smarthealthit-authentication
source_filename: smarthealthit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smarthealthit-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: smartOnFhir\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://launch.smarthealthit.org/v/r4/auth/authorize\n    tokenUrl: https://launch.smarthealthit.org/v/r4/auth/token\n    scopes: 6\n  - flow: clientCredentials\n    tokenUrl: https://launch.smarthealthit.org/v/r4/auth/token\n    scopes: 1\n  description: HL7 SMART App Launch OAuth 2.0 profile, used by the launcher's protected FHIR\n    proxy. The open r4.smarthealthit.org sandbox requires no authentication; the Bulk Data server\n    uses SMART Backend Services (client_credentials with a signed JWT assertion).\n  sources:\n  - openapi/smarthealthit-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smarthealthit/refs/heads/main/authentication/smarthealthit-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- SMART on FHIR
- FHIR
- Health IT
- EHR Integration
- Clinical Data
- Clinical Records
- Patient Facing
- Open Standards
- Interoperability
---
