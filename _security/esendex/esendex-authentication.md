---
anonymous_access: false
api_key_in: []
api_specs:
- filename: esendex-credential-management-api-openapi.yml
  format: yaml
  label: Esendex Credential Management API
  slug: esendex-credential-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esendex/refs/heads/main/openapi/esendex-credential-management-api-openapi.yml
- filename: esendex-message-dispatcher-api-openapi.yml
  format: yaml
  label: Esendex Message Dispatcher API
  slug: esendex-message-dispatcher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esendex/refs/heads/main/openapi/esendex-message-dispatcher-api-openapi.yml
- filename: esendex-message-headers-api-openapi.yml
  format: yaml
  label: Esendex Message Headers API
  slug: esendex-message-headers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esendex/refs/heads/main/openapi/esendex-message-headers-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Esendex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Esendex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Esendex
provider_slug: esendex
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Enter a JWT token to authorize the requests...
  name: JWTBearerAuth
  scheme: Bearer
  sources:
  - openapi/esendex-openapi.json
  type: http
slug: esendex-authentication
source_filename: esendex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/esendex-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: JWTBearerAuth\n  type: http\n  scheme: Bearer\n  bearerFormat: JWT\n  description: Enter a JWT token to authorize the requests...\n  sources:\n  - openapi/esendex-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esendex/refs/heads/main/authentication/esendex-authentication.yml
summary_line: http · 1 scheme
tags:
- SMS
- Messaging
- Communications
- API
- Business
---
