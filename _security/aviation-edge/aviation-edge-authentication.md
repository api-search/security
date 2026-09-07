---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: aviation-edge-openapi.yml
  format: yaml
  label: Aviation Edge
  slug: aviation-edge
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aviation-edge/refs/heads/main/openapi/_original/aviation-edge-openapi.yml
- filename: aviation-edge-real-time-api-openapi.yml
  format: yaml
  label: Aviation Edge Real-Time API
  slug: aviation-edge-real-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aviation-edge/refs/heads/main/openapi/aviation-edge-real-time-api-openapi.yml
- filename: aviation-edge-reference-api-openapi.yml
  format: yaml
  label: Aviation Edge Reference API
  slug: aviation-edge-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aviation-edge/refs/heads/main/openapi/aviation-edge-reference-api-openapi.yml
- filename: aviation-edge-satellites-api-openapi.yml
  format: yaml
  label: Aviation Edge Satellites API
  slug: aviation-edge-satellites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aviation-edge/refs/heads/main/openapi/aviation-edge-satellites-api-openapi.yml
- filename: aviation-edge-schedules-api-openapi.yml
  format: yaml
  label: Aviation Edge Schedules API
  slug: aviation-edge-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aviation-edge/refs/heads/main/openapi/aviation-edge-schedules-api-openapi.yml
- filename: aviation-edge-notams-api-openapi.yml
  format: yaml
  label: Aviation Edge NOTAMs API
  slug: aviation-edge-notams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aviation-edge/refs/heads/main/openapi/aviation-edge-notams-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aviation Edge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aviation Edge secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aviation Edge
provider_slug: aviation-edge
scheme_count: 1
schemes:
- applies_to: all operations
  description: API key issued with an Aviation Edge subscription and passed as the `key` query parameter on every request, e.g. https://aviation-edge.com/v2/public/flights?key=YOUR_KEY&limit=100
  in: query
  name: ApiKeyAuth
  parameter: key
  required: true
  sources:
  - openapi/_original/aviation-edge-openapi.yml
  - https://aviation-edge.com/developers/
  type: apiKey
slug: aviation-edge-authentication
source_filename: aviation-edge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: >-\n  https://aviation-edge.com/developers/ and https://aviation-edge.com/free-api-key/, the\n  first-party request examples at https://github.com/AviationEdgeAPI, live probes of\n  https://aviation-edge.com/v2/public/ on 2026-09-04, and the securitySchemes declared in\n  openapi/_original/aviation-edge-openapi.yml.\ndocs: https://aviation-edge.com/developers/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  oauth: false\n  mtls: false\n  scopes: false\n  note: >-\n    One credential model, applied uniformly to all 17 operations: a subscription API key in\n    the `key` query parameter. There are no scopes, no header alternative, no OAuth surface\n    and no service accounts, so an agent's access is all-or-nothing per key.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: key\n  description: >-\n    API key issued with an Aviation Edge subscription and passed as the `key` query parameter\n\
  \    on every request, e.g. https://aviation-edge.com/v2/public/flights?key=YOUR_KEY&limit=100\n  required: true\n  applies_to: all operations\n  sources:\n  - openapi/_original/aviation-edge-openapi.yml\n  - https://aviation-edge.com/developers/\nkey_issuance:\n  self_serve: true\n  url: https://aviation-edge.com/premium-api/\n  free_tier: false\n  note: >-\n    Keys are issued on paid subscription and delivered by email and in the account dashboard\n    (https://aviation-edge.com/subscribe/login.php). The free API key was withdrawn — see\n    https://aviation-edge.com/free-api-key/ — so there is no anonymous or trial credential.\n  rotation: not documented\n  expiry: not documented\nfailure_modes:\n- condition: no key supplied\n  http_status: 200\n  body: '{\"message\":\"Missing API Key\",\"success\":false}'\n- condition: invalid key\n  http_status: 200\n  body: '{\"error\":\"Invalid API Key\",\"success\":false}'\n- note: >-\n    Authentication failures are returned with HTTP 200. A\
  \ client must inspect `success` in the\n    body; branching on the status code alone will read a rejected call as an empty result set.\n    See errors/aviation-edge-problem-types.yml.\ncautions:\n- >-\n    The credential travels in the query string, so it is exposed to server logs, proxy logs,\n    browser history and Referer headers. Aviation Edge offers no header-based alternative.\n- >-\n    Transport is TLS 1.3 with HSTS (see security/aviation-edge-domain-security.yml), so the key\n    is not exposed on the wire, only in whatever records the URL.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aviation-edge/refs/heads/main/authentication/aviation-edge-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Airlines
- Airports
- Aviation
- Flight Data
- Real-Time
---
