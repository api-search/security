---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: agent-module-dev-checkout-api-openapi.yml
  format: yaml
  label: Agent Module Checkout API
  slug: agent-module-dev-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-checkout-api-openapi.yml
- filename: agent-module-dev-delta-api-openapi.yml
  format: yaml
  label: Agent Module Delta API
  slug: agent-module-dev-delta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-delta-api-openapi.yml
- filename: agent-module-dev-demo-api-openapi.yml
  format: yaml
  label: Agent Module Demo API
  slug: agent-module-dev-demo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-demo-api-openapi.yml
- filename: agent-module-dev-interest-api-openapi.yml
  format: yaml
  label: Agent Module Interest API
  slug: agent-module-dev-interest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-interest-api-openapi.yml
- filename: agent-module-dev-keys-api-openapi.yml
  format: yaml
  label: Agent Module Keys API
  slug: agent-module-dev-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-keys-api-openapi.yml
- filename: agent-module-dev-mcp-api-openapi.yml
  format: yaml
  label: Agent Module MCP API
  slug: agent-module-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-mcp-api-openapi.yml
- filename: agent-module-dev-referral-api-openapi.yml
  format: yaml
  label: Agent Module Referral API
  slug: agent-module-dev-referral-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-referral-api-openapi.yml
- filename: agent-module-dev-status-api-openapi.yml
  format: yaml
  label: Agent Module Status API
  slug: agent-module-dev-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-status-api-openapi.yml
- filename: agent-module-dev-telemetry-api-openapi.yml
  format: yaml
  label: Agent Module Telemetry API
  slug: agent-module-dev-telemetry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-telemetry-api-openapi.yml
- filename: agent-module-dev-trial-api-openapi.yml
  format: yaml
  label: Agent Module Trial API
  slug: agent-module-dev-trial-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-trial-api-openapi.yml
- filename: agent-module-dev-verify-api-openapi.yml
  format: yaml
  label: Agent Module Verify API
  slug: agent-module-dev-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-verify-api-openapi.yml
- filename: agent-module-dev-waitlist-api-openapi.yml
  format: yaml
  label: Agent Module Waitlist API
  slug: agent-module-dev-waitlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-waitlist-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Agent Module Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agent Module secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Agent Module
provider_slug: agent-module-dev
scheme_count: 3
schemes:
- description: Agent Module membership key (am_live_ prefix) or trial key (am_trial_ prefix). Required for gated content layers.
  in: header
  name: ApiKeyHeader
  parameter: X-Agent-Module-Key
  sources:
  - openapi/agent-module-dev-openapi.json
  type: apiKey
- description: Skyfire PAY or KYA+PAY token for per-use access. $0.002 charged per content node request. Obtain from https://app.skyfire.xyz
  in: header
  name: SkyfirePayId
  parameter: skyfire-pay-id
  sources:
  - openapi/agent-module-dev-openapi.json
  type: apiKey
- description: Admin key for internal operations (key issuance, management). Set as ADMIN_KEY worker secret.
  name: AdminKey
  scheme: bearer
  sources:
  - openapi/agent-module-dev-openapi.json
  type: http
slug: agent-module-dev-authentication
source_filename: agent-module-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/agent-module-dev-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Agent-Module-Key\n  description: Agent Module membership key (am_live_ prefix) or trial key (am_trial_ prefix).\n    Required for gated content layers.\n  sources:\n  - openapi/agent-module-dev-openapi.json\n- name: SkyfirePayId\n  type: apiKey\n  in: header\n  parameter: skyfire-pay-id\n  description: Skyfire PAY or KYA+PAY token for per-use access. $0.002 charged per content node\n    request. Obtain from https://app.skyfire.xyz\n  sources:\n  - openapi/agent-module-dev-openapi.json\n- name: AdminKey\n  type: http\n  scheme: bearer\n  description: Admin key for internal operations (key issuance, management). Set as ADMIN_KEY\n    worker secret.\n  sources:\n  - openapi/agent-module-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/agent-module-dev/authentication/agent-module-dev-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Artificial Intelligence
- Automation
- Knowledge Base
- Agents
- Platform
---
