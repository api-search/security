---
api_key_in:
- header
api_specs:
- filename: accredible-analytics-api-openapi.yml
  format: yaml
  label: Accredible Analytics API
  slug: accredible-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-analytics-api-openapi.yml
- filename: accredible-credentials-api-openapi.yml
  format: yaml
  label: Accredible Credentials API
  slug: accredible-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-credentials-api-openapi.yml
- filename: accredible-departments-api-openapi.yml
  format: yaml
  label: Accredible Departments API
  slug: accredible-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-departments-api-openapi.yml
- filename: accredible-designs-api-openapi.yml
  format: yaml
  label: Accredible Designs API
  slug: accredible-designs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-designs-api-openapi.yml
- filename: accredible-evidence-items-api-openapi.yml
  format: yaml
  label: Accredible Evidence Items API
  slug: accredible-evidence-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-evidence-items-api-openapi.yml
- filename: accredible-groups-api-openapi.yml
  format: yaml
  label: Accredible Groups API
  slug: accredible-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-groups-api-openapi.yml
- filename: accredible-issuer-api-openapi.yml
  format: yaml
  label: Accredible Issuer API
  slug: accredible-issuer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-issuer-api-openapi.yml
- filename: accredible-references-api-openapi.yml
  format: yaml
  label: Accredible References API
  slug: accredible-references-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-references-api-openapi.yml
- filename: accredible-sso-api-openapi.yml
  format: yaml
  label: Accredible SSO API
  slug: accredible-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-sso-api-openapi.yml
- filename: accredible-team-members-api-openapi.yml
  format: yaml
  label: Accredible Team Members API
  slug: accredible-team-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-team-members-api-openapi.yml
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
