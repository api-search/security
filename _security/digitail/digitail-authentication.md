---
api_key_in: []
api_specs:
- filename: digitail-openapi.yml
  format: yaml
  label: Digitail Pets API
  slug: digitail-pets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-openapi.yml
- filename: digitail-openapi.yml
  format: yaml
  label: Digitail Pet Parents and Clients API
  slug: digitail-pet-parents-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-openapi.yml
- filename: digitail-openapi.yml
  format: yaml
  label: Digitail Appointments API
  slug: digitail-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-openapi.yml
- filename: digitail-openapi.yml
  format: yaml
  label: Digitail Clinical Records API
  slug: digitail-clinical-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-openapi.yml
- filename: digitail-openapi.yml
  format: yaml
  label: Digitail Labs API
  slug: digitail-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-openapi.yml
- filename: digitail-openapi.yml
  format: yaml
  label: Digitail Billing and Invoicing API
  slug: digitail-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-openapi.yml
- filename: digitail-openapi.yml
  format: yaml
  label: Digitail Clinics and Staff API
  slug: digitail-clinics-staff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-openapi.yml
- filename: digitail-openapi.yml
  format: yaml
  label: Digitail Client Communication API
  slug: digitail-client-communication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-openapi.yml
- filename: digitail-openapi.yml
  format: yaml
  label: Digitail Files API
  slug: digitail-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-openapi.yml
- filename: digitail-openapi.yml
  format: yaml
  label: Digitail Reports API
  slug: digitail-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Digitail Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Digitail secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Digitail
provider_slug: digitail
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization-code grant with PKCE. Bearer access token is long-lived; a refresh token is also returned.
  flows:
  - authorizationUrl: https://vet.digitail.io/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://vet.digitail.io/oauth/token
  name: oauth2
  sources:
  - openapi/digitail-openapi.yml
  type: oauth2
slug: digitail-authentication
source_filename: digitail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/digitail-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://vet.digitail.io/oauth/authorize\n    tokenUrl: https://vet.digitail.io/oauth/token\n    scopes: 0\n  description: OAuth 2.0 authorization-code grant with PKCE. Bearer access token is long-lived;\n    a refresh token is also returned.\n  sources:\n  - openapi/digitail-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/authentication/digitail-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Veterinary
- PIMS
- Practice Management
- Pets
- Healthcare
- Scheduling
- Billing
- SaaS
---
