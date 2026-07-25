---
api_key_in: []
api_specs:
- filename: petexec-authentication-api-openapi.yml
  format: yaml
  label: PetExec Authentication API
  slug: petexec-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-authentication-api-openapi.yml
- filename: petexec-boarding-api-openapi.yml
  format: yaml
  label: PetExec Boarding API
  slug: petexec-boarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-boarding-api-openapi.yml
- filename: petexec-calendar-api-openapi.yml
  format: yaml
  label: PetExec Calendar API
  slug: petexec-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-calendar-api-openapi.yml
- filename: petexec-company-api-openapi.yml
  format: yaml
  label: PetExec Company API
  slug: petexec-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-company-api-openapi.yml
- filename: petexec-credit-cards-api-openapi.yml
  format: yaml
  label: PetExec Credit Cards API
  slug: petexec-credit-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-credit-cards-api-openapi.yml
- filename: petexec-daycare-api-openapi.yml
  format: yaml
  label: PetExec Daycare API
  slug: petexec-daycare-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-daycare-api-openapi.yml
- filename: petexec-grooming-api-openapi.yml
  format: yaml
  label: PetExec Grooming API
  slug: petexec-grooming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-grooming-api-openapi.yml
- filename: petexec-owners-api-openapi.yml
  format: yaml
  label: PetExec Owners API
  slug: petexec-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-owners-api-openapi.yml
- filename: petexec-pets-api-openapi.yml
  format: yaml
  label: PetExec Pets API
  slug: petexec-pets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-pets-api-openapi.yml
- filename: petexec-profile-api-openapi.yml
  format: yaml
  label: PetExec Profile API
  slug: petexec-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-profile-api-openapi.yml
- filename: petexec-purchase-history-api-openapi.yml
  format: yaml
  label: PetExec Purchase History API
  slug: petexec-purchase-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-purchase-history-api-openapi.yml
- filename: petexec-reports-api-openapi.yml
  format: yaml
  label: PetExec Reports API
  slug: petexec-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-reports-api-openapi.yml
- filename: petexec-scheduled-services-api-openapi.yml
  format: yaml
  label: PetExec Scheduled Services API
  slug: petexec-scheduled-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-scheduled-services-api-openapi.yml
- filename: petexec-vaccinations-api-openapi.yml
  format: yaml
  label: PetExec Vaccinations API
  slug: petexec-vaccinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-vaccinations-api-openapi.yml
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
