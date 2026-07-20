---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Armorcode Authentication
name_suffix: Authentication
oauth_flows: []
overview: ArmorCode secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ArmorCode
provider_slug: armorcode
scheme_count: 1
schemes:
- description: The ArmorCode REST API requires a bearer API token in the Authorization header. Requesting the Spring springdoc OpenAPI document at https://app.armorcode.com/v3/api-docs without a token returns HTTP 401, confirming a token-gated API. Tokens are provisioned from the authenticated ArmorCode application (app.armorcode.com). EU tenants use eu.armorcode.com.
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - https://app.armorcode.com/v3/api-docs
  type: http
slug: armorcode-authentication
source_filename: armorcode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://app.armorcode.com/v3/api-docs\nsummary:\n  types: [http]\n  scheme: bearer\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  description: >-\n    The ArmorCode REST API requires a bearer API token in the Authorization\n    header. Requesting the Spring springdoc OpenAPI document at\n    https://app.armorcode.com/v3/api-docs without a token returns HTTP 401,\n    confirming a token-gated API. Tokens are provisioned from the authenticated\n    ArmorCode application (app.armorcode.com). EU tenants use eu.armorcode.com.\n  sources: [https://app.armorcode.com/v3/api-docs]\nnotes:\n- No public OpenAPI/securitySchemes could be retrieved (auth-gated); auth model asserted from the live 401 response and ArmorCode's API-token model.\n- No OAuth2 authorization-server metadata found at /.well-known/oauth-authorization-server or /openid-configuration\
  \ (HTTP 403 on app host).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/armorcode/refs/heads/main/authentication/armorcode-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Application Security
- Vulnerability Management
- ASPM
- Exposure Management
- DevSecOps
- Compliance
- API
---
