---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Urban Sky Authentication
name_suffix: Authentication
oauth_flows: []
overview: Urban Sky secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Urban Sky
provider_slug: urban-sky
scheme_count: 1
schemes:
- description: Organization-scoped Urban Sky API token. Passed as apiToken to UrbanSkySDK.init() for the WebSocket telemetry feed, and as the x-api-token header on REST calls to https://api.ops.atmosys.com.
  in: header
  issuance: Contact Urban Sky support (support@atmosys.com); token delivered via secure email
  name: apiToken
  parameter: x-api-token
  sources:
  - https://docs.urbansky.com/guide/getting-started.html
  - https://docs.urbansky.com/api/javascript.html
  type: apiKey
slug: urban-sky-authentication
source_filename: urban-sky-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://docs.urbansky.com/guide/getting-started.html\nsource: https://docs.urbansky.com/guide/getting-started.html\nnotes: >-\n  No self-serve sign-up: API tokens are issued by contacting Urban Sky support\n  with organization details and delivered via secure email. Tokens are scoped\n  to the organization and grant access to that organization's balloon data.\n  Docs instruct server-side use only (never client-side, never committed to\n  version control). The SDK is initialized with the token (apiToken) and the\n  REST test endpoint takes it in the x-api-token header.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\nschemes:\n  - name: apiToken\n    type: apiKey\n    in: header\n    parameter: x-api-token\n    description: >-\n      Organization-scoped Urban Sky API token. Passed as apiToken to\n      UrbanSkySDK.init() for the WebSocket telemetry feed, and as the\n      x-api-token header on REST calls to https://api.ops.atmosys.com.\n\
  \    issuance: Contact Urban Sky support (support@atmosys.com); token delivered via secure email\n    sources:\n      - https://docs.urbansky.com/guide/getting-started.html\n      - https://docs.urbansky.com/api/javascript.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urban-sky/refs/heads/main/authentication/urban-sky-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Aerospace
- Stratospheric Balloons
- Remote Sensing
- Earth Observation
- Aerial Imagery
- Telemetry
- Defense
- Weather
---
