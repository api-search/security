---
api_key_in: []
api_specs:
- filename: roivant-sciences-allergies-api-openapi.yml
  format: yaml
  label: Roivant Sciences Allergies API
  slug: roivant-sciences-allergies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-allergies-api-openapi.yml
- filename: roivant-sciences-appointments-api-openapi.yml
  format: yaml
  label: Roivant Sciences Appointments API
  slug: roivant-sciences-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-appointments-api-openapi.yml
- filename: roivant-sciences-diagnoses-api-openapi.yml
  format: yaml
  label: Roivant Sciences Diagnoses API
  slug: roivant-sciences-diagnoses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-diagnoses-api-openapi.yml
- filename: roivant-sciences-documents-api-openapi.yml
  format: yaml
  label: Roivant Sciences Documents API
  slug: roivant-sciences-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-documents-api-openapi.yml
- filename: roivant-sciences-encounters-api-openapi.yml
  format: yaml
  label: Roivant Sciences Encounters API
  slug: roivant-sciences-encounters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-encounters-api-openapi.yml
- filename: roivant-sciences-immunizations-api-openapi.yml
  format: yaml
  label: Roivant Sciences Immunizations API
  slug: roivant-sciences-immunizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-immunizations-api-openapi.yml
- filename: roivant-sciences-labs-api-openapi.yml
  format: yaml
  label: Roivant Sciences Labs API
  slug: roivant-sciences-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-labs-api-openapi.yml
- filename: roivant-sciences-medications-api-openapi.yml
  format: yaml
  label: Roivant Sciences Medications API
  slug: roivant-sciences-medications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-medications-api-openapi.yml
- filename: roivant-sciences-patients-api-openapi.yml
  format: yaml
  label: Roivant Sciences Patients API
  slug: roivant-sciences-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-patients-api-openapi.yml
- filename: roivant-sciences-practices-api-openapi.yml
  format: yaml
  label: Roivant Sciences Practices API
  slug: roivant-sciences-practices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-practices-api-openapi.yml
- filename: roivant-sciences-procedures-api-openapi.yml
  format: yaml
  label: Roivant Sciences Procedures API
  slug: roivant-sciences-procedures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-procedures-api-openapi.yml
- filename: roivant-sciences-providers-api-openapi.yml
  format: yaml
  label: Roivant Sciences Providers API
  slug: roivant-sciences-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-providers-api-openapi.yml
- filename: roivant-sciences-vitals-api-openapi.yml
  format: yaml
  label: Roivant Sciences Vitals API
  slug: roivant-sciences-vitals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-vitals-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Roivant Sciences Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Roivant Sciences secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Roivant Sciences
provider_slug: roivant-sciences
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://api.healthjump.com/oauth/token
  name: OAuth2
  sources:
  - openapi/datavant-healthjump-ehr-openapi.yml
  type: oauth2
slug: roivant-sciences-authentication
source_filename: roivant-sciences-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/datavant-healthjump-ehr-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.healthjump.com/oauth/token\n    scopes: 3\n  sources:\n  - openapi/datavant-healthjump-ehr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/authentication/roivant-sciences-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Biotech
- Pharmaceuticals
- Drug Development
- Clinical Trials
- Health Data
- Tokenization
- Electronic Health Records
- Real World Evidence
- Holding Company
- Healthcare
---
