---
api_key_in:
- header
api_specs:
- filename: valgo-compute-api-openapi.yml
  format: yaml
  label: Valgo Compute API
  slug: valgo-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valgo/refs/heads/main/openapi/valgo-compute-api-openapi.yml
- filename: valgo-compute-batch-api-openapi.yml
  format: yaml
  label: Valgo Compute Batch API
  slug: valgo-compute-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valgo/refs/heads/main/openapi/valgo-compute-batch-api-openapi.yml
- filename: valgo-compute-depot-route-api-openapi.yml
  format: yaml
  label: Valgo Compute Depot Route API
  slug: valgo-compute-depot-route-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valgo/refs/heads/main/openapi/valgo-compute-depot-route-api-openapi.yml
- filename: valgo-compute-route-api-openapi.yml
  format: yaml
  label: Valgo Compute Route API
  slug: valgo-compute-route-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valgo/refs/heads/main/openapi/valgo-compute-route-api-openapi.yml
- filename: valgo-health-api-openapi.yml
  format: yaml
  label: Valgo Health API
  slug: valgo-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valgo/refs/heads/main/openapi/valgo-health-api-openapi.yml
- filename: valgo-manifest-api-openapi.yml
  format: yaml
  label: Valgo Manifest API
  slug: valgo-manifest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valgo/refs/heads/main/openapi/valgo-manifest-api-openapi.yml
- filename: valgo-request-api-key-api-openapi.yml
  format: yaml
  label: Valgo Request Api Key API
  slug: valgo-request-api-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valgo/refs/heads/main/openapi/valgo-request-api-key-api-openapi.yml
- filename: valgo-v1-api-openapi.yml
  format: yaml
  label: Valgo v1 API
  slug: valgo-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valgo/refs/heads/main/openapi/valgo-v1-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Valgo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Valgo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Valgo
provider_slug: valgo
scheme_count: 1
schemes:
- description: The versioned public surface under /v1 is API-key-authenticated; keys are sent via the X-API-Key header (quoted from the API's own OpenAPI info.description). Keys use the hbk_ prefix and the official Python client reads them from the HUMANBASELINES_API_KEY environment variable. Keys are requested via the POST /request-api-key operation (operationId request_api_key_request_api_key_post).
  environment_variable: HUMANBASELINES_API_KEY
  in: header
  key_prefix: hbk_
  name: X-API-Key
  parameter: X-API-Key
  sources:
  - openapi/valgo-humanbaselines-openapi.json
  type: apiKey
slug: valgo-authentication
source_filename: valgo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/valgorithmic/humanbaselines (README) + https://humanbaselines.com/openapi.json (info.description)\ndocs: https://docs.humanbaselines.com\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  key_prefix: hbk_\n  environment_variable: HUMANBASELINES_API_KEY\n  description: >-\n    The versioned public surface under /v1 is API-key-authenticated; keys are\n    sent via the X-API-Key header (quoted from the API's own OpenAPI\n    info.description). Keys use the hbk_ prefix and the official Python\n    client reads them from the HUMANBASELINES_API_KEY environment variable.\n    Keys are requested via the POST /request-api-key operation\n    (operationId request_api_key_request_api_key_post).\n  sources:\n  - openapi/valgo-humanbaselines-openapi.json\nnotes: >-\n  The OpenAPI document itself declares no components.securitySchemes;\
  \ the\n  auth model above is taken from the provider's published README and the\n  spec's info.description. Missing 401 responses / securitySchemes in the\n  spec are flagged in overlays/valgo-humanbaselines-overlay.yaml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valgo/refs/heads/main/authentication/valgo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Insurance
- Risk Management
- Autonomous Vehicles
- Robotics
- Artificial Intelligence
- Safety Validation
- Actuarial
---
