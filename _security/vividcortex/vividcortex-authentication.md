---
api_key_in:
- header
api_specs:
- filename: vividcortex-openapi.yml
  format: yaml
  label: VividCortex Database Performance Monitor API
  slug: vividcortex-database-performance-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vividcortex/refs/heads/main/openapi/vividcortex-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Vividcortex Authentication
name_suffix: Authentication
oauth_flows: []
overview: VividCortex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: VividCortex
provider_slug: vividcortex
scheme_count: 1
schemes:
- description: 'Per-environment API token passed as `Authorization: Bearer <API_TOKEN>`. Created in DPM Settings → API Tokens; role-based (RBAC). Agent tokens are explicitly discouraged for API use.'
  format: Bearer <API_TOKEN>
  header: Authorization
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/vividcortex-openapi.yml
  type: http
slug: vividcortex-authentication
source_filename: vividcortex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/vividcortex-openapi.yml\ndocs: https://docs.vividcortex.com/api/basics/api-tokens/\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  notes: >-\n    The v2 REST API authenticates with a per-environment Bearer API token created in the\n    DPM web app under Settings → API Tokens. Tokens are role-scoped (RBAC) and should be\n    treated as secrets; compromised tokens can be rotated from the API Tokens page. The\n    token's environment scopes every call — there is no separate tenant/account parameter.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Per-environment API token passed as `Authorization: Bearer <API_TOKEN>`. Created in\n    DPM Settings → API Tokens; role-based (RBAC). Agent tokens are explicitly discouraged\n    for API use.\n  header: Authorization\n  format: \"Bearer <API_TOKEN>\"\n  sources:\n  - openapi/vividcortex-openapi.yml\napp_authentication:\n  note:\
  \ >-\n    The DPM web application (distinct from the API) supports email/password login plus\n    Google and GitHub OAuth, optional mandatory OAuth for a G Suite/GitHub org, and SAML\n    SSO (Okta, OneLogin, Azure AD) for Premium-tier organizations. The API itself uses\n    only the Bearer API token above — there is no OAuth2/OIDC client flow for API access.\n  docs: https://docs.vividcortex.com/general-reference/authentication/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vividcortex/refs/heads/main/authentication/vividcortex-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Database
- Performance Monitoring
- Observability
- Monitoring
- APM
- Database Performance
- SQL
- DevOps
- SolarWinds
---
