---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Opsera Authentication
name_suffix: Authentication
oauth_flows: []
overview: Opsera secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Opsera
provider_slug: opsera
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Opsera Personal Access Tokens are standard JWT bearer tokens generated in the Opsera Portal (Profile -> Access Tokens). Each token is created with a predefined scope, an expiration date, and is owned by the generating user; all API calls apply that user''s RBAC. A Power User (or higher) role is required for list operations; individual object actions are evaluated against the object''s RBAC. Tokens are never stored by Opsera (only metadata) and can be expired early. Validation layers: authentic+active token -> valid owner -> not de-activated -> scope match -> object-level access. Failure returns HTTP 403 Forbidden.'
  example: 'Authorization: Bearer <token>'
  header: Authorization
  in: header
  name: opseraPersonalAccessToken
  scheme: bearer
  sources:
  - docs
  type: http
slug: opsera-authentication
source_filename: opsera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.opsera.io/api-platform-and-integration/opsera-api-platform/personal-access-tokens\ndocs: https://docs.opsera.io/api-platform-and-integration/opsera-api-platform/personal-access-tokens\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  bearer_format: JWT\n  token_model: personal-access-token\n  api_key_in: [header]\nschemes:\n  - name: opseraPersonalAccessToken\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    in: header\n    header: Authorization\n    example: 'Authorization: Bearer <token>'\n    description: >-\n      Opsera Personal Access Tokens are standard JWT bearer tokens generated in the Opsera Portal\n      (Profile -> Access Tokens). Each token is created with a predefined scope, an expiration date,\n      and is owned by the generating user; all API calls apply that user's RBAC. A Power User (or\n      higher) role is required for list operations; individual object actions are evaluated\
  \ against\n      the object's RBAC. Tokens are never stored by Opsera (only metadata) and can be expired early.\n      Validation layers: authentic+active token -> valid owner -> not de-activated -> scope match ->\n      object-level access. Failure returns HTTP 403 Forbidden.\n    sources: [docs]\nsso:\n  - Okta (SAML/OIDC)\n  - Azure AD (Entra ID) SSO\n  - SCIM-based user provisioning (Azure)\nnotes: >-\n  The interactive portal (portal.opsera.io) authenticates end users via Okta / enterprise SSO;\n  programmatic REST + MCP access uses JWT bearer Personal Access Tokens.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opsera/refs/heads/main/authentication/opsera-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- DevOps
- CI/CD
- DevSecOps
- Pipeline Orchestration
- Developer Tools
- Software Delivery
- Governance
- MCP
- AI Agents
---
