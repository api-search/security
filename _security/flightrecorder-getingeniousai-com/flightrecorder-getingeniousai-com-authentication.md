---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: flightrecorder-getingeniousai-com-actions-api-openapi.yml
  format: yaml
  label: Agent Flight Recorder (Ingenious AI) Actions API
  slug: flightrecorder-getingeniousai-com-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightrecorder-getingeniousai-com/openapi/flightrecorder-getingeniousai-com-actions-api-openapi.yml
- filename: flightrecorder-getingeniousai-com-agents-api-openapi.yml
  format: yaml
  label: Agent Flight Recorder (Ingenious AI) Agents API
  slug: flightrecorder-getingeniousai-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightrecorder-getingeniousai-com/openapi/flightrecorder-getingeniousai-com-agents-api-openapi.yml
- filename: flightrecorder-getingeniousai-com-attestations-api-openapi.yml
  format: yaml
  label: Agent Flight Recorder (Ingenious AI) Attestations API
  slug: flightrecorder-getingeniousai-com-attestations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightrecorder-getingeniousai-com/openapi/flightrecorder-getingeniousai-com-attestations-api-openapi.yml
- filename: flightrecorder-getingeniousai-com-audit-api-openapi.yml
  format: yaml
  label: Agent Flight Recorder (Ingenious AI) Audit API
  slug: flightrecorder-getingeniousai-com-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightrecorder-getingeniousai-com/openapi/flightrecorder-getingeniousai-com-audit-api-openapi.yml
- filename: flightrecorder-getingeniousai-com-chain-api-openapi.yml
  format: yaml
  label: Agent Flight Recorder (Ingenious AI) Chain API
  slug: flightrecorder-getingeniousai-com-chain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightrecorder-getingeniousai-com/openapi/flightrecorder-getingeniousai-com-chain-api-openapi.yml
- filename: flightrecorder-getingeniousai-com-checkpoints-api-openapi.yml
  format: yaml
  label: Agent Flight Recorder (Ingenious AI) Checkpoints API
  slug: flightrecorder-getingeniousai-com-checkpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightrecorder-getingeniousai-com/openapi/flightrecorder-getingeniousai-com-checkpoints-api-openapi.yml
- filename: flightrecorder-getingeniousai-com-cost-attestations-api-openapi.yml
  format: yaml
  label: Agent Flight Recorder (Ingenious AI) Cost Attestations API
  slug: flightrecorder-getingeniousai-com-cost-attestations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightrecorder-getingeniousai-com/openapi/flightrecorder-getingeniousai-com-cost-attestations-api-openapi.yml
- filename: flightrecorder-getingeniousai-com-inclusion-api-openapi.yml
  format: yaml
  label: Agent Flight Recorder (Ingenious AI) Inclusion API
  slug: flightrecorder-getingeniousai-com-inclusion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightrecorder-getingeniousai-com/openapi/flightrecorder-getingeniousai-com-inclusion-api-openapi.yml
- filename: flightrecorder-getingeniousai-com-negative-proofs-api-openapi.yml
  format: yaml
  label: Agent Flight Recorder (Ingenious AI) Negative Proofs API
  slug: flightrecorder-getingeniousai-com-negative-proofs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightrecorder-getingeniousai-com/openapi/flightrecorder-getingeniousai-com-negative-proofs-api-openapi.yml
- filename: flightrecorder-getingeniousai-com-otel-api-openapi.yml
  format: yaml
  label: Agent Flight Recorder (Ingenious AI) Otel API
  slug: flightrecorder-getingeniousai-com-otel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightrecorder-getingeniousai-com/openapi/flightrecorder-getingeniousai-com-otel-api-openapi.yml
- filename: flightrecorder-getingeniousai-com-oversight-api-openapi.yml
  format: yaml
  label: Agent Flight Recorder (Ingenious AI) Oversight API
  slug: flightrecorder-getingeniousai-com-oversight-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightrecorder-getingeniousai-com/openapi/flightrecorder-getingeniousai-com-oversight-api-openapi.yml
- filename: flightrecorder-getingeniousai-com-run-seals-api-openapi.yml
  format: yaml
  label: Agent Flight Recorder (Ingenious AI) Run Seals API
  slug: flightrecorder-getingeniousai-com-run-seals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightrecorder-getingeniousai-com/openapi/flightrecorder-getingeniousai-com-run-seals-api-openapi.yml
- filename: flightrecorder-getingeniousai-com-runs-api-openapi.yml
  format: yaml
  label: Agent Flight Recorder (Ingenious AI) Runs API
  slug: flightrecorder-getingeniousai-com-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightrecorder-getingeniousai-com/openapi/flightrecorder-getingeniousai-com-runs-api-openapi.yml
- filename: flightrecorder-getingeniousai-com-usage-api-openapi.yml
  format: yaml
  label: Agent Flight Recorder (Ingenious AI) Usage API
  slug: flightrecorder-getingeniousai-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightrecorder-getingeniousai-com/openapi/flightrecorder-getingeniousai-com-usage-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Agent Flight Recorder (Ingenious AI) Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agent Flight Recorder (Ingenious AI) secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Agent Flight Recorder (Ingenious AI)
provider_slug: flightrecorder-getingeniousai-com
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/admt-getingeniousai-com-openapi.json
  - openapi/agentblock-getingeniousai-com-openapi.json
  type: apiKey
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/agentgate-getingeniousai-com-openapi.json
  - openapi/flightrecorder-getingeniousai-com-openapi.json
  type: http
slug: flightrecorder-getingeniousai-com-authentication
source_filename: flightrecorder-getingeniousai-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/admt-getingeniousai-com-openapi.json, openapi/agentblock-getingeniousai-com-openapi.json,\n  openapi/agentgate-getingeniousai-com-openapi.json, openapi/flightrecorder-getingeniousai-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/admt-getingeniousai-com-openapi.json\n  - openapi/agentblock-getingeniousai-com-openapi.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/agentgate-getingeniousai-com-openapi.json\n  - openapi/flightrecorder-getingeniousai-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/flightrecorder-getingeniousai-com/authentication/flightrecorder-getingeniousai-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Artificial Intelligence
- Audit
- Logging
- Compliance
- Platform
---
