---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cambio-uruguay-aduana-api-openapi.yml
  format: yaml
  label: Cambio Uruguay Aduana API
  slug: cambio-uruguay-aduana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-uruguay/refs/heads/main/openapi/cambio-uruguay-aduana-api-openapi.yml
- filename: cambio-uruguay-ai-insights-api-openapi.yml
  format: yaml
  label: Cambio Uruguay AI Insights API
  slug: cambio-uruguay-ai-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-uruguay/refs/heads/main/openapi/cambio-uruguay-ai-insights-api-openapi.yml
- filename: cambio-uruguay-banks-api-openapi.yml
  format: yaml
  label: Cambio Uruguay Banks API
  slug: cambio-uruguay-banks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-uruguay/refs/heads/main/openapi/cambio-uruguay-banks-api-openapi.yml
- filename: cambio-uruguay-bcu-api-openapi.yml
  format: yaml
  label: Cambio Uruguay BCU API
  slug: cambio-uruguay-bcu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-uruguay/refs/heads/main/openapi/cambio-uruguay-bcu-api-openapi.yml
- filename: cambio-uruguay-debug-api-openapi.yml
  format: yaml
  label: Cambio Uruguay Debug API
  slug: cambio-uruguay-debug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-uruguay/refs/heads/main/openapi/cambio-uruguay-debug-api-openapi.yml
- filename: cambio-uruguay-evolution-api-openapi.yml
  format: yaml
  label: Cambio Uruguay Evolution API
  slug: cambio-uruguay-evolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-uruguay/refs/heads/main/openapi/cambio-uruguay-evolution-api-openapi.yml
- filename: cambio-uruguay-exchange-data-api-openapi.yml
  format: yaml
  label: Cambio Uruguay Exchange Data API
  slug: cambio-uruguay-exchange-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-uruguay/refs/heads/main/openapi/cambio-uruguay-exchange-data-api-openapi.yml
- filename: cambio-uruguay-geocoding-api-openapi.yml
  format: yaml
  label: Cambio Uruguay Geocoding API
  slug: cambio-uruguay-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-uruguay/refs/heads/main/openapi/cambio-uruguay-geocoding-api-openapi.yml
- filename: cambio-uruguay-health-api-openapi.yml
  format: yaml
  label: Cambio Uruguay Health API
  slug: cambio-uruguay-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-uruguay/refs/heads/main/openapi/cambio-uruguay-health-api-openapi.yml
- filename: cambio-uruguay-indicators-api-openapi.yml
  format: yaml
  label: Cambio Uruguay Indicators API
  slug: cambio-uruguay-indicators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-uruguay/refs/heads/main/openapi/cambio-uruguay-indicators-api-openapi.yml
- filename: cambio-uruguay-locations-api-openapi.yml
  format: yaml
  label: Cambio Uruguay Locations API
  slug: cambio-uruguay-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-uruguay/refs/heads/main/openapi/cambio-uruguay-locations-api-openapi.yml
- filename: cambio-uruguay-parameters-api-openapi.yml
  format: yaml
  label: Cambio Uruguay Parameters API
  slug: cambio-uruguay-parameters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-uruguay/refs/heads/main/openapi/cambio-uruguay-parameters-api-openapi.yml
- filename: cambio-uruguay-regional-api-openapi.yml
  format: yaml
  label: Cambio Uruguay Regional API
  slug: cambio-uruguay-regional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-uruguay/refs/heads/main/openapi/cambio-uruguay-regional-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: derived
name: Cambio Uruguay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cambio Uruguay declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Cambio Uruguay
provider_slug: cambio-uruguay
scheme_count: 0
schemes: []
slug: cambio-uruguay-authentication
source_filename: cambio-uruguay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: derived\nsource: openapi/cambio-uruguay-openapi.json + live probes of https://api.cambio-uruguay.com and https://mcp.cambio-uruguay.com/mcp, 2026-09-07\nsummary: >-\n  No authentication, by design. The OpenAPI declares no securitySchemes and no security\n  requirements; the API answered unauthenticated GETs live (200 on / and\n  /evolution/brou/USD, 2026-09-07); the MCP server completed initialize + tools/list with\n  no credentials; and the site's llms.txt describes the service as a free public tool with\n  no key or registration. This is a genuinely keyless public API, not an undocumented\n  auth gap.\nschemes: []\nauth_required: false\nsignup_required: false\napi_key: null\noauth2: null\nevidence:\n- url: https://api.cambio-uruguay.com/\n  status: 200\n  note: unauthenticated request returned live rates JSON\n- url: https://api.cambio-uruguay.com/evolution/brou/USD\n  status: 200\n  note: unauthenticated request returned 370-point historical\
  \ series\n- url: https://mcp.cambio-uruguay.com/mcp\n  status: 200\n  note: anonymous MCP initialize + tools/list handshake completed\nagent_note: >-\n  An agent can call every documented operation with zero onboarding — no key issuance,\n  no OAuth flow, no signup. The /debug/* and POST /cache/flush operations are also\n  unauthenticated per the spec; they are operational endpoints and agents should not\n  call them.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cambio-uruguay/refs/heads/main/authentication/cambio-uruguay-authentication.yml
summary_line: 0 schemes
tags:
- Currency
- Exchange Rates
- Finance
- Uruguay
- Latin America
- MCP
- Agent-Native
- Open Source
---
