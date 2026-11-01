---
anonymous_access: false
api_key_in: []
api_specs:
- filename: grabbit-live-account-api-openapi.yml
  format: yaml
  label: grabbit-live Account API
  slug: grabbit-live-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grabbit-live/openapi/grabbit-live-account-api-openapi.yml
- filename: grabbit-live-grabs-api-openapi.yml
  format: yaml
  label: grabbit-live Grabs API
  slug: grabbit-live-grabs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grabbit-live/openapi/grabbit-live-grabs-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Grabbit Live Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: grabbit-live secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: grabbit-live
provider_slug: grabbit-live
scheme_count: 2
schemes:
- description: API key from https://grabbit.live/app/api-keys. sk_live_ keys render real screenshots and spend credits; sk_test_ keys return free placeholders.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/grabbit-live-openapi.json
  - openapi/www.grabbit.live_openapi.json
  type: http
- description: OAuth 2.1 authorization code + PKCE with dynamic client registration (RFC 7591). Used by MCP clients such as claude.ai.
  flows:
  - authorizationUrl: https://www.grabbit.live/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://www.grabbit.live/api/v1/oauth/token
  name: oauth2
  sources:
  - openapi/grabbit-live-openapi.json
  - openapi/www.grabbit.live_openapi.json
  type: oauth2
slug: grabbit-live-authentication
source_filename: grabbit-live-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/grabbit-live-openapi.json, openapi/www.grabbit.live_openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key from https://grabbit.live/app/api-keys. sk_live_ keys render real screenshots\n    and spend credits; sk_test_ keys return free placeholders.\n  sources:\n  - openapi/grabbit-live-openapi.json\n  - openapi/www.grabbit.live_openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.grabbit.live/oauth/authorize\n    tokenUrl: https://www.grabbit.live/api/v1/oauth/token\n    scopes: 1\n  description: OAuth 2.1 authorization code + PKCE with dynamic client registration (RFC 7591).\n    Used by MCP clients such as claude.ai.\n  sources:\n  - openapi/grabbit-live-openapi.json\n  - openapi/www.grabbit.live_openapi.json\n"
source_yaml_url: https://artifacts.apis.io/grabbit-live/authentication/grabbit-live-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Screenshot
- AI-Agent
- Automation
- API
- Visual
---
