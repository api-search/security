---
api_key_in:
- header
api_specs:
- filename: reefapi-openapi.json
  format: json
  label: ReefAPI REST API
  slug: reefapi-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reefapi/refs/heads/main/openapi/reefapi-openapi.json
auth_types:
- apiKey
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Reefapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: ReefAPI secures its APIs with apiKey and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ReefAPI
provider_slug: reefapi
scheme_count: 2
schemes:
- applies_to: all 1528 operations (declared as a global `security` requirement in the OpenAPI)
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/reefapi-openapi.json
  - https://reefapi.com/docs
  surface: REST
  type: apiKey
- applies_to: the call_engine tool only
  header: Authorization
  name: BearerKey
  note: 'The MCP server takes the SAME ReefAPI key but as ''Authorization: Bearer <key>'', not as x-api-key. Not declared in the OpenAPI (the MCP endpoint is outside the spec).'
  scheme: bearer
  sources:
  - https://reefapi.com/mcp
  - https://reefapi.com/llms.txt
  surface: MCP (https://api.reefapi.com/mcp)
  type: http
slug: reefapi-authentication
source_filename: reefapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-31'\nmethod: searched\nsource: https://reefapi.com/docs (Authentication section) + https://reefapi.com/mcp + openapi/reefapi-openapi.json + live 401 probe 2026-08-31\ndocs: https://reefapi.com/docs\nname: ReefAPI\nslug: reefapi\nsummary:\n  model: single-credential, no OAuth, no scopes\n  types:\n  - apiKey\n  - http-bearer\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mtls: false\n  note: >-\n    One key covers the entire 183-engine catalog and the MCP server — there is no\n    per-engine credential, no scope surface and no token exchange. The same key is\n    presented two different ways depending on the surface, which is the one thing an\n    integrator has to get right.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  surface: REST\n  applies_to: all 1528 operations (declared as a global `security` requirement in the OpenAPI)\n  sources:\n  - openapi/reefapi-openapi.json\n  - https://reefapi.com/docs\n\
  - name: BearerKey\n  type: http\n  scheme: bearer\n  header: Authorization\n  surface: MCP (https://api.reefapi.com/mcp)\n  applies_to: the call_engine tool only\n  sources:\n  - https://reefapi.com/mcp\n  - https://reefapi.com/llms.txt\n  note: >-\n    The MCP server takes the SAME ReefAPI key but as 'Authorization: Bearer <key>',\n    not as x-api-key. Not declared in the OpenAPI (the MCP endpoint is outside the spec).\nkey_management:\n  issued_from: https://reefapi.com/signup (dashboard)\n  prefix: ak_live_\n  display_policy: full key shown once at creation\n  rotation_documented: false\n  guidance: \"Keep it server-side; never ship it to a browser. (docs, Authentication section)\"\nanonymous_access:\n  rest: false\n  mcp_discovery: true\n  detail: >-\n    PROBED 2026-08-31. The MCP methods initialize, tools/list, prompts/list and\n    resources/list all return 200 with no Authorization header. Four of the five tools\n    (search_engines, get_catalog, get_engine_schema, get_action_schema)\
  \ are documented\n    and verified keyless. Only call_engine authenticates and spends credits. The\n    OpenAPI itself (https://api.reefapi.com/openapi.json) and the RFC 9727 api-catalog\n    are also anonymous.\nfailure_behavior:\n  status: 401\n  code: AUTH_FAILED\n  envelope: '{\"ok\":false,\"meta\":{...},\"error\":{\"code\":\"AUTH_FAILED\",\"message\":\"auth: no_key\",\"retryable\":false}}'\n  observed: '2026-08-31 POST https://api.reefapi.com/currency/v1/convert with no key'\n  note: The 401 body is the standard success envelope with ok=false — error semantics are uniform with the happy path.\ngaps:\n- \"No /.well-known/openid-configuration, /.well-known/oauth-authorization-server or /.well-known/oauth-protected-resource on either host (all 404) — the MCP server is key-auth, not OAuth-protected, so RFC 9728 protected-resource metadata does not apply.\"\n- \"No documented key-rotation or key-expiry policy.\"\n- \"No IP allow-listing, per-key scope restriction or read-only key variant\
  \ is documented.\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reefapi/refs/heads/main/authentication/reefapi-authentication.yml
summary_line: apiKey/http-bearer · 2 schemes
tags:
- web-data
- data-aggregation
- web-scraping
- serp
- e-commerce
- social-media
- real-estate
- jobs
- travel
- news
- finance
- reviews
- company-intelligence
- mcp
- agent-native
- rest
- openapi
- llms-txt
- api-catalog
- free-tier
- credits
- gateway
---
