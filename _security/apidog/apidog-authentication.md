---
api_key_in: []
api_specs:
- filename: apidog-apidog-openapi.yml
  format: yaml
  label: Apidog
  slug: apidog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apidog/refs/heads/main/openapi/apidog-apidog-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apidog Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apidog secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apidog
provider_slug: apidog
scheme_count: 1
schemes:
- description: Apidog API uses Bearer Token authorization. Include your personal API access token in the Authorization header as "Bearer {token}". Tokens are generated under Avatar -> Account Settings -> API Access Token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/apidog-apidog-openapi.yml
  type: http
slug: apidog-authentication
source_filename: apidog-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apidog-apidog-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Apidog API uses Bearer Token authorization. Include your personal API access\n    token in the Authorization header as \"Bearer {token}\". Tokens are generated under Avatar\n    -> Account Settings -> API Access Token.\n  sources:\n  - openapi/apidog-apidog-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apidog/refs/heads/main/authentication/apidog-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Coding
- API Design
- API Lifecycle
- API Testing
- Collaboration
- Design-First
- Documentation
- MCP
- Mocking
- Platform
---
