---
api_key_in: []
api_specs:
- filename: digitail-appointments-api-openapi.yml
  format: yaml
  label: Digitail Appointments API
  slug: digitail-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-appointments-api-openapi.yml
- filename: digitail-breeds-api-openapi.yml
  format: yaml
  label: Digitail Breeds API
  slug: digitail-breeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-breeds-api-openapi.yml
- filename: digitail-charges-api-openapi.yml
  format: yaml
  label: Digitail Charges API
  slug: digitail-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-charges-api-openapi.yml
- filename: digitail-clients-api-openapi.yml
  format: yaml
  label: Digitail Clients API
  slug: digitail-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-clients-api-openapi.yml
- filename: digitail-clinics-api-openapi.yml
  format: yaml
  label: Digitail Clinics API
  slug: digitail-clinics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-clinics-api-openapi.yml
- filename: digitail-files-api-openapi.yml
  format: yaml
  label: Digitail Files API
  slug: digitail-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-files-api-openapi.yml
- filename: digitail-invoices-api-openapi.yml
  format: yaml
  label: Digitail Invoices API
  slug: digitail-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-invoices-api-openapi.yml
- filename: digitail-labs-api-openapi.yml
  format: yaml
  label: Digitail Labs API
  slug: digitail-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-labs-api-openapi.yml
- filename: digitail-medication-api-openapi.yml
  format: yaml
  label: Digitail Medication API
  slug: digitail-medication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-medication-api-openapi.yml
- filename: digitail-pet-parents-api-openapi.yml
  format: yaml
  label: Digitail Pet Parents API
  slug: digitail-pet-parents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-pet-parents-api-openapi.yml
- filename: digitail-pets-api-openapi.yml
  format: yaml
  label: Digitail Pets API
  slug: digitail-pets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-pets-api-openapi.yml
- filename: digitail-prescriptions-api-openapi.yml
  format: yaml
  label: Digitail Prescriptions API
  slug: digitail-prescriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-prescriptions-api-openapi.yml
- filename: digitail-records-api-openapi.yml
  format: yaml
  label: Digitail Records API
  slug: digitail-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-records-api-openapi.yml
- filename: digitail-reports-api-openapi.yml
  format: yaml
  label: Digitail Reports API
  slug: digitail-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-reports-api-openapi.yml
- filename: digitail-sales-api-openapi.yml
  format: yaml
  label: Digitail Sales API
  slug: digitail-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-sales-api-openapi.yml
- filename: digitail-species-api-openapi.yml
  format: yaml
  label: Digitail Species API
  slug: digitail-species-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-species-api-openapi.yml
- filename: digitail-vets-api-openapi.yml
  format: yaml
  label: Digitail Vets API
  slug: digitail-vets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-vets-api-openapi.yml
- filename: digitail-visit-types-api-openapi.yml
  format: yaml
  label: Digitail Visit Types API
  slug: digitail-visit-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-visit-types-api-openapi.yml
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
