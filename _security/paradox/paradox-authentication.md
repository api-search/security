---
api_key_in: []
api_specs:
- filename: paradox-authentication-api-openapi.yml
  format: yaml
  label: Paradox Authentication API
  slug: paradox-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-authentication-api-openapi.yml
- filename: paradox-candidate-attributes-api-openapi.yml
  format: yaml
  label: Paradox Candidate Attributes API
  slug: paradox-candidate-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-candidate-attributes-api-openapi.yml
- filename: paradox-candidates-api-openapi.yml
  format: yaml
  label: Paradox Candidates API
  slug: paradox-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-candidates-api-openapi.yml
- filename: paradox-company-api-openapi.yml
  format: yaml
  label: Paradox Company API
  slug: paradox-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-company-api-openapi.yml
- filename: paradox-location-areas-api-openapi.yml
  format: yaml
  label: Paradox Location Areas API
  slug: paradox-location-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-location-areas-api-openapi.yml
- filename: paradox-location-rooms-api-openapi.yml
  format: yaml
  label: Paradox Location Rooms API
  slug: paradox-location-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-location-rooms-api-openapi.yml
- filename: paradox-locations-api-openapi.yml
  format: yaml
  label: Paradox Locations API
  slug: paradox-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-locations-api-openapi.yml
- filename: paradox-reporting-api-openapi.yml
  format: yaml
  label: Paradox Reporting API
  slug: paradox-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-reporting-api-openapi.yml
- filename: paradox-scheduling-api-openapi.yml
  format: yaml
  label: Paradox Scheduling API
  slug: paradox-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-scheduling-api-openapi.yml
- filename: paradox-user-permissions-api-openapi.yml
  format: yaml
  label: Paradox User Permissions API
  slug: paradox-user-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-user-permissions-api-openapi.yml
- filename: paradox-users-api-openapi.yml
  format: yaml
  label: Paradox Users API
  slug: paradox-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-users-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Paradox Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Paradox secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Paradox
provider_slug: paradox
scheme_count: 2
schemes:
- description: OAuth 2.0 client credentials authentication
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /auth/token
  name: oauth2
  sources:
  - openapi/paradox-api-openapi.yml
  type: oauth2
- bearerFormat: JWT
  description: Bearer token obtained from the OAuth 2.0 token endpoint
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/paradox-api-openapi.yml
  type: http
slug: paradox-authentication
source_filename: paradox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/paradox-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/token\n    scopes: 0\n  description: OAuth 2.0 client credentials authentication\n  sources:\n  - openapi/paradox-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token obtained from the OAuth 2.0 token endpoint\n  sources:\n  - openapi/paradox-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/authentication/paradox-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Artificial Intelligence
- Candidate Screening
- Chatbot
- Conversational AI
- Hiring Automation
- HR Technology
- Interview Scheduling
- Recruiting
- SMS
- Talent Acquisition
---
