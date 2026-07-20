---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Devrev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Devrev secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Devrev
provider_slug: devrev
scheme_count: 1
schemes:
- description: DevRev authenticates API requests with a Personal Access Token (PAT) created from within the DevRev app (Settings > Account > Personal Access Tokens). The PAT is sent as a Bearer token in the Authorization header; the raw token value alone in Authorization is also accepted.
  format: 'Authorization: Bearer <PAT>'
  header: Authorization
  in: header
  name: PersonalAccessToken
  scheme: bearer
  type: http
slug: devrev-authentication
source_filename: devrev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.devrev.ai/about/authentication\ndocs: https://developer.devrev.ai/about/authentication\nsummary:\n  types: [http]\n  scheme: bearer\n  token_kind: personal-access-token\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: PersonalAccessToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: \"Authorization: Bearer <PAT>\"\n  description: >-\n    DevRev authenticates API requests with a Personal Access Token (PAT)\n    created from within the DevRev app (Settings > Account > Personal Access\n    Tokens). The PAT is sent as a Bearer token in the Authorization header;\n    the raw token value alone in Authorization is also accepted.\ntoken_management:\n  create: PATs are minted in the DevRev web app.\n  service_accounts: >-\n    Service-account tokens and auth-tokens/auth-connections endpoints exist for\n    snap-ins and machine-to-machine access (see the auth-tokens\
  \ and\n    auth-connections API groups).\nnotes: >-\n  No user-facing OAuth 2.0 authorization-code flow or scope catalog is documented\n  for the public REST API, so scopes/ is intentionally omitted (PAT-only auth).\n  Snap-ins use keyrings/auth-connections to hold third-party credentials.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/devrev/refs/heads/main/authentication/devrev-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Customer Support
- Product Development
- Issue Tracking
- Knowledge Base
- CRM
- Developer Tools
- AI
- Webhooks
- Automation
---
