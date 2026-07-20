---
api_key_in: []
api_specs:
- filename: petexec-openapi.yml
  format: yaml
  label: PetExec Owners API
  slug: petexec-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-openapi.yml
- filename: petexec-openapi.yml
  format: yaml
  label: PetExec Pets API
  slug: petexec-pets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-openapi.yml
- filename: petexec-openapi.yml
  format: yaml
  label: PetExec Reservations API
  slug: petexec-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-openapi.yml
- filename: petexec-openapi.yml
  format: yaml
  label: PetExec Calendar API
  slug: petexec-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-openapi.yml
- filename: petexec-openapi.yml
  format: yaml
  label: PetExec Services API
  slug: petexec-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-openapi.yml
- filename: petexec-openapi.yml
  format: yaml
  label: PetExec Vaccinations API
  slug: petexec-vaccinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-openapi.yml
- filename: petexec-openapi.yml
  format: yaml
  label: PetExec Billing & Reports API
  slug: petexec-billing-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-openapi.yml
- filename: petexec-openapi.yml
  format: yaml
  label: PetExec Company & Account API
  slug: petexec-company-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Petexec Authentication
name_suffix: Authentication
oauth_flows: []
overview: PetExec secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PetExec
provider_slug: petexec
scheme_count: 1
schemes:
- description: 'OAuth2 password-grant access token obtained from POST /token. Passed as `Authorization: Bearer [example key]`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/petexec-openapi.yml
  type: http
slug: petexec-authentication
source_filename: petexec-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/petexec-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'OAuth2 password-grant access token obtained from POST /token. Passed as `Authorization:\n    Bearer [example key]`.'\n  sources:\n  - openapi/petexec-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/authentication/petexec-authentication.yml
summary_line: http · 1 scheme
tags:
- Pet Care
- Boarding
- Daycare
- Grooming
- Training
- Business Management
- Pet Business Software
---
