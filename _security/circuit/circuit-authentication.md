---
api_key_in: []
api_specs:
- filename: circuit-depots-api-openapi.yml
  format: yaml
  label: Circuit Depots API
  slug: circuit-depots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-depots-api-openapi.yml
- filename: circuit-drivers-api-openapi.yml
  format: yaml
  label: Circuit Drivers API
  slug: circuit-drivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-drivers-api-openapi.yml
- filename: circuit-live-plans-api-openapi.yml
  format: yaml
  label: Circuit Live Plans API
  slug: circuit-live-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-live-plans-api-openapi.yml
- filename: circuit-live-stops-api-openapi.yml
  format: yaml
  label: Circuit Live Stops API
  slug: circuit-live-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-live-stops-api-openapi.yml
- filename: circuit-members-api-openapi.yml
  format: yaml
  label: Circuit Members API
  slug: circuit-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-members-api-openapi.yml
- filename: circuit-operations-api-openapi.yml
  format: yaml
  label: Circuit Operations API
  slug: circuit-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-operations-api-openapi.yml
- filename: circuit-plans-api-openapi.yml
  format: yaml
  label: Circuit Plans API
  slug: circuit-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-plans-api-openapi.yml
- filename: circuit-routes-api-openapi.yml
  format: yaml
  label: Circuit Routes API
  slug: circuit-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-routes-api-openapi.yml
- filename: circuit-stops-api-openapi.yml
  format: yaml
  label: Circuit Stops API
  slug: circuit-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-stops-api-openapi.yml
- filename: circuit-team-api-openapi.yml
  format: yaml
  label: Circuit Team API
  slug: circuit-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-team-api-openapi.yml
- filename: circuit-unassigned-stops-api-openapi.yml
  format: yaml
  label: Circuit Unassigned Stops API
  slug: circuit-unassigned-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-unassigned-stops-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Circuit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Circuit secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Circuit
provider_slug: circuit
scheme_count: 2
schemes:
- description: Primary scheme. Use the API key as the username with an empty password, base64-encoded, e.g. `curl https://api.spoke.com/public/v1/plans -u yourApiKey:`.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/circuit-v0.2b-openapi-original.json
  - openapi/circuit-v1-openapi-original.json
  type: http
- description: 'Alternative scheme documented in the API docs (not declared in the OpenAPI securitySchemes). Pass the API key with no encoding as `Authorization: Bearer yourApiKey`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - https://developer.dispatch.spoke.com/api/v1
  type: http
slug: circuit-authentication
source_filename: circuit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/circuit-v1-openapi-original.json\ndocs: https://developer.dispatch.spoke.com/api/v1\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  - bearer\n  api_key_delivery: >-\n    A single API key generated in Spoke Dispatch settings > Integrations > API.\n    The same key is presented either via HTTP Basic (key as username, empty\n    password, base64-encoded) or as a Bearer token in the Authorization header.\n  notes:\n  - HTTPS is required; plain HTTP requests are rejected.\n  - Every request with a body must send Content-Type application/json.\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: >-\n    Primary scheme. Use the API key as the username with an empty password,\n    base64-encoded, e.g. `curl https://api.spoke.com/public/v1/plans -u yourApiKey:`.\n  sources:\n  - openapi/circuit-v0.2b-openapi-original.json\n  - openapi/circuit-v1-openapi-original.json\n- name: BearerAuth\n\
  \  type: http\n  scheme: bearer\n  description: >-\n    Alternative scheme documented in the API docs (not declared in the OpenAPI\n    securitySchemes). Pass the API key with no encoding as\n    `Authorization: Bearer yourApiKey`.\n  sources:\n  - https://developer.dispatch.spoke.com/api/v1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/authentication/circuit-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Delivery
- Logistics
- Last Mile
- Route Optimization
- Dispatch
- Couriers
- Fleet
- Proof of Delivery
- Field Service
---
