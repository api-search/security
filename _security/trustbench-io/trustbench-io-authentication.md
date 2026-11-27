---
anonymous_access: false
api_key_in: []
api_specs:
- filename: trustbench-io-receipts-api-openapi.yml
  format: yaml
  label: TrustBench Receipts API
  slug: trustbench-io-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trustbench-io/openapi/trustbench-io-receipts-api-openapi.yml
- filename: trustbench-io-routing-api-openapi.yml
  format: yaml
  label: TrustBench Routing API
  slug: trustbench-io-routing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trustbench-io/openapi/trustbench-io-routing-api-openapi.yml
- filename: trustbench-io-telemetry-api-openapi.yml
  format: yaml
  label: TrustBench Telemetry API
  slug: trustbench-io-telemetry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trustbench-io/openapi/trustbench-io-telemetry-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: TrustBench Authentication
name_suffix: Authentication
oauth_flows: []
overview: TrustBench secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TrustBench
provider_slug: trustbench-io
scheme_count: 1
schemes:
- bearerFormat: tb_live_<argon2id-key>
  description: Server-side API key. Used as the auth fallback on POST /route when the x402 paywall is disabled, and for POST /route/settle.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/trustbench-io-openapi.json
  type: http
slug: trustbench-io-authentication
source_filename: trustbench-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: derived\nsource: openapi/trustbench-io-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: tb_live_<argon2id-key>\n  description: Server-side API key. Used as the auth fallback on POST /route when the x402 paywall\n    is disabled, and for POST /route/settle.\n  sources:\n  - openapi/trustbench-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/trustbench-io/authentication/trustbench-io-authentication.yml
summary_line: http · 1 scheme
tags:
- FinTech
- Payments
- Blockchain
- Registry
- Telemetry
---
