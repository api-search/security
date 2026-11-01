---
anonymous_access: false
api_key_in: []
api_specs:
- filename: blinkinbox-club-account-api-openapi.yml
  format: yaml
  label: blinkinbox-club Account API
  slug: blinkinbox-club-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkinbox-club/openapi/blinkinbox-club-account-api-openapi.yml
- filename: blinkinbox-club-domains-api-openapi.yml
  format: yaml
  label: blinkinbox-club Domains API
  slug: blinkinbox-club-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkinbox-club/openapi/blinkinbox-club-domains-api-openapi.yml
- filename: blinkinbox-club-inboxes-api-openapi.yml
  format: yaml
  label: blinkinbox-club Inboxes API
  slug: blinkinbox-club-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkinbox-club/openapi/blinkinbox-club-inboxes-api-openapi.yml
- filename: blinkinbox-club-messages-api-openapi.yml
  format: yaml
  label: blinkinbox-club Messages API
  slug: blinkinbox-club-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkinbox-club/openapi/blinkinbox-club-messages-api-openapi.yml
- filename: blinkinbox-club-webhooks-api-openapi.yml
  format: yaml
  label: blinkinbox-club Webhooks API
  slug: blinkinbox-club-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkinbox-club/openapi/blinkinbox-club-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Blinkinbox Club Authentication
name_suffix: Authentication
oauth_flows: []
overview: blinkinbox-club secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: blinkinbox-club
provider_slug: blinkinbox-club
scheme_count: 1
schemes:
- description: API key from the dashboard, e.g. `bb_live_...`. `X-API-Key` header also works.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/blinkinbox-club-openapi.json
  type: http
slug: blinkinbox-club-authentication
source_filename: blinkinbox-club-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/blinkinbox-club-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key from the dashboard, e.g. `bb_live_...`. `X-API-Key` header also works.\n  sources:\n  - openapi/blinkinbox-club-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/blinkinbox-club/authentication/blinkinbox-club-authentication.yml
summary_line: http · 1 scheme
tags:
- Email
- Temporary
- API
- MCP
- DeveloperTools
- Disposable
---
