---
api_key_in: []
api_specs:
- filename: swoogo-openapi.yml
  format: yaml
  label: Swoogo Events API
  slug: swoogo-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swoogo/refs/heads/main/openapi/swoogo-openapi.yml
- filename: swoogo-openapi.yml
  format: yaml
  label: Swoogo Registrants API
  slug: swoogo-registrants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swoogo/refs/heads/main/openapi/swoogo-openapi.yml
- filename: swoogo-openapi.yml
  format: yaml
  label: Swoogo Sessions API
  slug: swoogo-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swoogo/refs/heads/main/openapi/swoogo-openapi.yml
- filename: swoogo-openapi.yml
  format: yaml
  label: Swoogo Speakers API
  slug: swoogo-speakers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swoogo/refs/heads/main/openapi/swoogo-openapi.yml
- filename: swoogo-openapi.yml
  format: yaml
  label: Swoogo Contacts API
  slug: swoogo-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swoogo/refs/heads/main/openapi/swoogo-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Swoogo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Swoogo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Swoogo
provider_slug: swoogo
scheme_count: 1
schemes:
- description: Bearer token obtained from POST /oauth2/token using the OAuth2 client_credentials grant. Tokens expire every 30 minutes.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/swoogo-openapi.yml
  type: http
slug: swoogo-authentication
source_filename: swoogo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/swoogo-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained from POST /oauth2/token using the OAuth2 client_credentials\n    grant. Tokens expire every 30 minutes.\n  sources:\n  - openapi/swoogo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swoogo/refs/heads/main/authentication/swoogo-authentication.yml
summary_line: http · 1 scheme
tags:
- Event Management
- Event Registration
- Events
- Sessions
- Speakers
- Attendees
- SaaS
---
