---
api_key_in: []
api_specs:
- filename: accept-midas-openapi-original.yml
  format: yaml
  label: MIDAS API
  slug: midas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accept/refs/heads/main/openapi/accept-midas-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Accept Authentication
name_suffix: Authentication
oauth_flows: []
overview: Accept secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Accept
provider_slug: accept
scheme_count: 1
schemes:
- description: Static bearer token on the Authorization header for all /v1/* routes. Configured via MIDAS_AUTH_TOKENS or midas.yaml auth.tokens as "token|principal-id|role1,role2" (semicolon-separated for multiple; supports ${VAR} expansion). Not required when auth.mode=open (logs "UNSAFE FOR PRODUCTION" — development only).
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/accept-midas-openapi-original.yml
  type: http
slug: accept-authentication
source_filename: accept-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/accept-midas-openapi-original.yml + docs/guides/authentication.md\ndocs: https://github.com/accept-io/midas/blob/main/docs/guides/authentication.md\nsummary:\n  types:\n  - http\n  http_scheme: bearer\n  modes:\n  - open\n  - required\n  - oidc\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Static bearer token on the Authorization header for all /v1/* routes. Configured via\n    MIDAS_AUTH_TOKENS or midas.yaml auth.tokens as \"token|principal-id|role1,role2\"\n    (semicolon-separated for multiple; supports ${VAR} expansion). Not required when\n    auth.mode=open (logs \"UNSAFE FOR PRODUCTION\" — development only).\n  sources:\n  - openapi/accept-midas-openapi-original.yml\nmodes:\n- id: open\n  description: No authentication required. Default; logs UNSAFE FOR PRODUCTION at startup. Local development only.\n- id: required\n  description: Enforces bearer-token validation on all\
  \ governed /v1/* routes.\n- id: oidc\n  description: OIDC/SSO for Explorer browser access only (provider-agnostic — issuer_url, client_id/secret, redirect_url, username_claim, groups_claim, role_mappings). Separate from API auth.\nrbac:\n  note: Bearer principals and OIDC groups map to internal roles.\n  roles:\n  - platform.admin\n  - platform.operator\n  - platform.viewer\n  - governance.approver\n  - governance.reviewer\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accept/refs/heads/main/authentication/accept-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Enterprise
- Governance
- AI Agents
- Authority
- Decision Governance
- Audit
- Open Source
---
