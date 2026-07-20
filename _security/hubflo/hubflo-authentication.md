---
api_key_in: []
api_specs:
- filename: hubflo-openapi-original.yml
  format: yaml
  label: Hubflo API
  slug: hubflo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubflo/refs/heads/main/openapi/hubflo-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Hubflo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hubflo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hubflo
provider_slug: hubflo
scheme_count: 1
schemes:
- format: Bearer <token>
  header: Authorization
  name: bearer_auth
  scheme: bearer
  sources:
  - openapi/hubflo-openapi-original.yml
  type: http
slug: hubflo-authentication
source_filename: hubflo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/hubflo-openapi-original.yml\ndocs: https://hubflo.readme.io/reference/token-authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\nschemes:\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  header: Authorization\n  format: 'Bearer <token>'\n  sources:\n  - openapi/hubflo-openapi-original.yml\ndocs_detail: >-\n  Hubflo uses bearer (token) authentication. Send the authentication token in the\n  Authorization header as 'Authorization: Bearer <token>'. Generate the API key in Hubflo\n  under Settings > Integrations (app.hubflo.com/organizations). The key is shared across all\n  members of the organization. Use POST /api/v2/pings to verify an authenticated request.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hubflo/refs/heads/main/authentication/hubflo-authentication.yml
summary_line: http · 1 scheme
tags:
- Client Portal
- Professional Services
- CRM
- Invoicing
- Project Management
- Document Management
- E-Signature
- Onboarding
- Webhooks
- Company
---
