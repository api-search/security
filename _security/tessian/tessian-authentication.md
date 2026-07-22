---
api_key_in:
- header
api_specs:
- filename: tessian-openapi-original.json
  format: json
  label: Tessian API
  slug: tessian-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/openapi/tessian-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Tessian Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tessian secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tessian
provider_slug: tessian
scheme_count: 1
schemes:
- description: A Tessian portal user with "Logs" permission generates an API Token under Integrations > Tessian API in the portal. The token is shown only once at creation. It inherits the permissions of the creating user and is automatically revoked if that user is removed or loses the Logs permission, or when the token is deleted.
  format: 'Authorization: API-Token <your-api-token>'
  header_name: Authorization
  in: header
  name: api-token
  sources:
  - openapi/tessian-openapi-original.json
  type: apiKey
slug: tessian-authentication
source_filename: tessian-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.tessian.com/documentation/api/index.html\ndocs: https://developer.tessian.com/documentation/api/index.html\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  note: >-\n    The Tessian API uses a static API Token passed in the Authorization header.\n    The OpenAPI document does not declare a components.securitySchemes entry;\n    this profile is captured from the provider's published authentication docs.\nschemes:\n- name: api-token\n  type: apiKey\n  in: header\n  header_name: Authorization\n  format: 'Authorization: API-Token <your-api-token>'\n  sources:\n  - openapi/tessian-openapi-original.json\n  description: >-\n    A Tessian portal user with \"Logs\" permission generates an API Token under\n    Integrations > Tessian API in the portal. The token is shown only once at\n    creation. It inherits the permissions of the creating user and is\n    automatically revoked if that\
  \ user is removed or loses the Logs permission,\n    or when the token is deleted.\ntoken_lifecycle:\n  shown_once: true\n  inherits_user_permissions: true\n  required_permission: Logs\n  auto_revoked_when:\n  - user removed\n  - Logs permission revoked\n  - token deleted\n  system_account_supported: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/authentication/tessian-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Enterprise
- Email Security
- Cybersecurity
- Data Loss Prevention
- SIEM
- Security
- Phishing
---
