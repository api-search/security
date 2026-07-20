---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Adverity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adverity secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Adverity
provider_slug: adverity
scheme_count: 2
schemes:
- description: 'API keys generated programmatically via POST https://{{INSTANCE}}/api/auth/token/ (username + password). The token does not expire and is only rotated when the account password is deliberately changed. Sent as `Authorization: Token {{KEY}}`.'
  format: Token {{KEY}}
  in: header
  name: ManagementApiToken
  parameter: Authorization
  sources:
  - docs
  type: apiKey
- description: 'API keys generated in the Adverity UI (Administration > Management API keys). Limited to 5 per workspace, require Administrator permissions in the root workspace, do not expire, and can be rotated via POST https://{{INSTANCE}}/api/v1/auth/keys/current/rotate/. Sent as `Authorization: Bearer {{KEY}}`.'
  format: Bearer {{KEY}}
  in: header
  name: ManagementApiBearer
  parameter: Authorization
  sources:
  - docs
  type: apiKey
slug: adverity-authentication
source_filename: adverity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://docs.adverity.com/guides/management-api/authorizing-to-management-api.html\ndocs: https://docs.adverity.com/guides/management-api/authorizing-to-management-api.html\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    The Adverity Management API uses long-lived API-key (token) authentication in\n    the Authorization header. There is no OAuth2 for the Management API itself;\n    OAuth is used only downstream when Adverity authorizes to connected data\n    sources (Google Ads, Facebook Ads, LinkedIn Ads, etc.) on the user's behalf.\nschemes:\n- name: ManagementApiToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Token {{KEY}}'\n  description: >-\n    API keys generated programmatically via POST https://{{INSTANCE}}/api/auth/token/\n    (username + password). The token does not expire and is only rotated when the\n    account password is deliberately changed.\
  \ Sent as `Authorization: Token {{KEY}}`.\n  sources: [docs]\n- name: ManagementApiBearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Bearer {{KEY}}'\n  description: >-\n    API keys generated in the Adverity UI (Administration > Management API keys).\n    Limited to 5 per workspace, require Administrator permissions in the root\n    workspace, do not expire, and can be rotated via\n    POST https://{{INSTANCE}}/api/v1/auth/keys/current/rotate/. Sent as\n    `Authorization: Bearer {{KEY}}`.\n  sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adverity/refs/heads/main/authentication/adverity-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Data Analytics
- Marketing Analytics
- Data Integration
- ETL
- Business Intelligence
- Marketing Intelligence
- MCP
---
