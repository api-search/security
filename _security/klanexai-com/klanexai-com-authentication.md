---
anonymous_access: false
api_key_in: []
api_specs:
- filename: klanexai-com-api-key-api-openapi.yml
  format: yaml
  label: Klanex Api Key API
  slug: klanexai-com-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klanexai-com/openapi/klanexai-com-api-key-api-openapi.yml
- filename: klanexai-com-auth-api-openapi.yml
  format: yaml
  label: Klanex Auth API
  slug: klanexai-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klanexai-com/openapi/klanexai-com-auth-api-openapi.yml
- filename: klanexai-com-connections-api-openapi.yml
  format: yaml
  label: Klanex Connections API
  slug: klanexai-com-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klanexai-com/openapi/klanexai-com-connections-api-openapi.yml
- filename: klanexai-com-dashboard-api-openapi.yml
  format: yaml
  label: Klanex Dashboard API
  slug: klanexai-com-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klanexai-com/openapi/klanexai-com-dashboard-api-openapi.yml
- filename: klanexai-com-executions-api-openapi.yml
  format: yaml
  label: Klanex Executions API
  slug: klanexai-com-executions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klanexai-com/openapi/klanexai-com-executions-api-openapi.yml
- filename: klanexai-com-healthz-api-openapi.yml
  format: yaml
  label: Klanex Healthz API
  slug: klanexai-com-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klanexai-com/openapi/klanexai-com-healthz-api-openapi.yml
- filename: klanexai-com-integrations-api-openapi.yml
  format: yaml
  label: Klanex Integrations API
  slug: klanexai-com-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klanexai-com/openapi/klanexai-com-integrations-api-openapi.yml
- filename: klanexai-com-openapi-yaml-api-openapi.yml
  format: yaml
  label: Klanex Openapi.yaml API
  slug: klanexai-com-openapi-yaml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klanexai-com/openapi/klanexai-com-openapi-yaml-api-openapi.yml
- filename: klanexai-com-replays-api-openapi.yml
  format: yaml
  label: Klanex Replays API
  slug: klanexai-com-replays-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klanexai-com/openapi/klanexai-com-replays-api-openapi.yml
- filename: klanexai-com-webhook-secret-api-openapi.yml
  format: yaml
  label: Klanex Webhook Secret API
  slug: klanexai-com-webhook-secret-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klanexai-com/openapi/klanexai-com-webhook-secret-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Klanex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Klanex declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Klanex
provider_slug: klanexai-com
scheme_count: 1
schemes:
- evidence: "curl https://api.klanex.dev/v1/executions -H \"X-API-Key: klx_…\" -d '{\n \"target\": { \"method\": \"POST\", \"url\": \"https://api.stripe.com/v1/refunds\" },\n \"payload\": { \"charge\": \"ch_123\", \"amount\": 500 },\n \"payload_schema\": { \"type\": \"object\", \"required\": [\"charge\",\"amount\"] },\n \"callback_url\": \"https://you.example.com/hooks/klanex\",\n \"max_attempts\": 5\n}'"
  header: X-API-Key
  how_to_obtain: Get your API key
  location: header
  name: API Key
  type: apiKey
slug: klanexai-com-authentication
source_filename: klanexai-com-authentication.yml
source_heading: Authentication Profile
source_url: https://api.klanexai.com/signup/
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api.klanexai.com/signup/\nsources:\n- https://api.klanexai.com/signup/\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: \"curl https://api.klanex.dev/v1/executions -H \\\"X-API-Key: klx_…\\\" -d '{\\n \\\"target\\\": { \\\"method\\\": \\\"POST\\\", \\\"url\\\": \\\"https://api.stripe.com/v1/refunds\\\"\\\n    \\ },\\n \\\"payload\\\": { \\\"charge\\\": \\\"ch_123\\\", \\\"amount\\\": 500 },\\n \\\"payload_schema\\\": { \\\"type\\\": \\\"object\\\", \\\"required\\\": [\\\"charge\\\",\\\"\\\n    amount\\\"] },\\n \\\"callback_url\\\": \\\"https://you.example.com/hooks/klanex\\\",\\n \\\"max_attempts\\\": 5\\n}'\"\n  location: header\n  header: X-API-Key\n  how_to_obtain: Get your API key\ndocs: https://api.klanexai.com/signup/\n"
source_yaml_url: https://artifacts.apis.io/klanexai-com/authentication/klanexai-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Execution
- Agents
- Integration
- Platform
---
