---
api_key_in: []
api_specs:
- filename: pomo-openapi.yml
  format: yaml
  label: Pomo Platform API
  slug: pomo-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomo/refs/heads/main/openapi/pomo-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: probed
name: Pomo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pomo secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Pomo
provider_slug: pomo
scheme_count: 2
schemes:
- applies_to_operations: 932
  declared: true
  evidence:
  - body: '{"status":"healthy","clerk_configured":true,"secret_key_configured":true}'
    http_status: 200
    url: https://api.usepomo.ai/api/auth/health
  - body: '{"detail":"Missing authorization token"}'
    http_status: 401
    url: https://api.usepomo.ai/api/auth/status
    www_authenticate: Bearer
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/pomo-openapi.yml
  token_issuer: Clerk
  type: http
- applies_to: /api/programmatic/v1/*
  declared: false
  evidence:
  - body: '{"detail":"API key required"}'
    http_status: 401
    url: https://api.usepomo.ai/api/programmatic/v1/hello
  in: unknown — header name not published
  lifecycle:
    create: POST /api/programmatic-keys (create_api_key_for_profile_api_programmatic_keys_post)
    expiry_field: ApiKeyCreateRequest.expires_at (date-time, optional)
    list: GET /api/programmatic-keys (list_api_keys_api_programmatic_keys_get)
    revoke: POST /api/programmatic-keys/{api_key_id}/revoke
    scopes_field: ApiKeyCreateRequest.scopes (array of string; no scope vocabulary published)
    usage: GET /api/programmatic-keys/{api_key_id}/usage
  name: ProgrammaticApiKey
  type: apiKey
slug: pomo-authentication
source_filename: pomo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://api.usepomo.ai/openapi.json + live 401 probes of api.usepomo.ai\nnote: 'The OpenAPI declares exactly one securityScheme (HTTPBearer, http/bearer) applied to 932 of 994\n  operations. Live probing shows two distinct credential families behind that single declared scheme:\n  session bearer tokens issued by Clerk for the application surface, and opaque API keys for the /api/programmatic/v1\n  tier. The spec does not model the API-key scheme, so it is recorded here from observed 401 behaviour\n  rather than from the contract.'\nsummary:\n  types:\n  - http\n  - apiKey\n  declared_in_spec:\n  - http\n  observed_only:\n  - apiKey\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  declared: true\n  applies_to_operations: 932\n  sources:\n  - openapi/pomo-openapi.yml\n  token_issuer: Clerk\n  evidence:\n  - url: https://api.usepomo.ai/api/auth/health\n    http_status: 200\n    body: '{\"status\":\"healthy\",\"clerk_configured\"\
  :true,\"secret_key_configured\":true}'\n  - url: https://api.usepomo.ai/api/auth/status\n    http_status: 401\n    www_authenticate: Bearer\n    body: '{\"detail\":\"Missing authorization token\"}'\n- name: ProgrammaticApiKey\n  type: apiKey\n  declared: false\n  in: unknown — header name not published\n  applies_to: /api/programmatic/v1/*\n  lifecycle:\n    create: POST /api/programmatic-keys (create_api_key_for_profile_api_programmatic_keys_post)\n    list: GET /api/programmatic-keys (list_api_keys_api_programmatic_keys_get)\n    revoke: POST /api/programmatic-keys/{api_key_id}/revoke\n    usage: GET /api/programmatic-keys/{api_key_id}/usage\n    scopes_field: ApiKeyCreateRequest.scopes (array of string; no scope vocabulary published)\n    expiry_field: ApiKeyCreateRequest.expires_at (date-time, optional)\n  evidence:\n  - url: https://api.usepomo.ai/api/programmatic/v1/hello\n    http_status: 401\n    body: '{\"detail\":\"API key required\"}'\ntenancy:\n  header: X-Organization-Id\n\
  \  operations: 59\n  note: Organization scoping is carried as an X-Organization-Id header on 59 operations; most resource\n    operations additionally require company_profile_id.\n  secondary_header: X-Company-Profile-Id\npublic_operations:\n  count: 62\n  note: '62 operations declare no security: OAuth callbacks for connected platforms, inbound partner webhooks,\n    health endpoints, public pricing/plans, the latest ToS, social-post platform constraints, and the\n    discovery files (/robots.txt, /llms.txt, /sitemap.xml).'\nanonymous_discovery:\n  oauth_authorization_server: 404\n  oauth_protected_resource: 404\n  openid_configuration: 404\n  note: No RFC 8414 / RFC 9728 metadata is served on either host; see well-known/pomo-well-known.yml.\ngaps:\n- No published authentication documentation, developer portal, or key-issuance guide.\n- The API-key scheme is not declared in the OpenAPI, so an agent reading only the contract cannot authenticate\n  to the programmatic tier.\n- No scope\
  \ vocabulary is published for the ApiKeyCreateRequest.scopes field.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pomo/refs/heads/main/authentication/pomo-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Marketing
- AI
- Market Intelligence
- Competitive Intelligence
- Marketing Automation
- Generative AI
- SaaS
- Answer Engine Optimization
- Advertising
- Social Media
- Influencer Marketing
- Campaign Management
---
