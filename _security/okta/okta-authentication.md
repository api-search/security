---
api_key_in:
- header
api_specs:
- filename: okta-openapi-original.yml
  format: yaml
  label: Okta API
  slug: okta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okta/refs/heads/main/openapi/okta-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Okta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Okta secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Okta
provider_slug: okta
scheme_count: 1
schemes:
- description: SSWS {API Token}
  in: header
  name: api_token
  parameter: Authorization
  sources:
  - openapi/okta-openapi-original.yml
  type: apiKey
slug: okta-authentication
source_filename: okta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/okta-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: SSWS {API Token}\n  sources:\n  - openapi/okta-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/okta/refs/heads/main/authentication/okta-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Identity
- Workforce Identity
- Customer Identity
- Authentication
- Authorization
- Single Sign-On
- Multi-Factor Authentication
- Identity Governance
- Privileged Access
- AI Agents
- Cross-App Access
- MCP
- Platform
---
