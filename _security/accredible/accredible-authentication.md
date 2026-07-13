---
api_key_in:
- header
api_specs:
- filename: accredible-openapi.yml
  format: yaml
  label: Accredible Credentials API
  slug: accredible-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-openapi.yml
- filename: accredible-openapi.yml
  format: yaml
  label: Accredible Groups API
  slug: accredible-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-openapi.yml
- filename: accredible-openapi.yml
  format: yaml
  label: Accredible Designs API
  slug: accredible-designs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-openapi.yml
- filename: accredible-openapi.yml
  format: yaml
  label: Accredible Evidence and References API
  slug: accredible-evidence-references-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-openapi.yml
- filename: accredible-openapi.yml
  format: yaml
  label: Accredible Analytics API
  slug: accredible-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-openapi.yml
- filename: accredible-openapi.yml
  format: yaml
  label: Accredible Departments and Team Members API
  slug: accredible-departments-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-openapi.yml
- filename: accredible-openapi.yml
  format: yaml
  label: Accredible Issuer and SSO API
  slug: accredible-issuer-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Accredible Authentication
name_suffix: Authentication
oauth_flows: []
overview: Accredible secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Accredible
provider_slug: accredible
scheme_count: 1
schemes:
- description: API key sent in the Authorization header using the scheme `Token token=YOUR_API_KEY`.
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/accredible-openapi.yml
  type: apiKey
slug: accredible-authentication
source_filename: accredible-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/accredible-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key sent in the Authorization header using the scheme `Token token=YOUR_API_KEY`.\n  sources:\n  - openapi/accredible-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/authentication/accredible-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Digital Credentials
- Certificates
- Badges
- Open Badges
- Credentialing
- Verification
- Digital Badges
---
