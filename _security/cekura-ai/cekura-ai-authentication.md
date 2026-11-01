---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cekura-ai-ai-agents-api-openapi.yml
  format: yaml
  label: Cekura AI Agents API
  slug: cekura-ai-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cekura-ai/openapi/cekura-ai-ai-agents-api-openapi.yml
- filename: cekura-ai-call-logs-api-openapi.yml
  format: yaml
  label: Cekura Call Logs API
  slug: cekura-ai-call-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cekura-ai/openapi/cekura-ai-call-logs-api-openapi.yml
- filename: cekura-ai-dashboards-api-openapi.yml
  format: yaml
  label: Cekura Dashboards API
  slug: cekura-ai-dashboards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cekura-ai/openapi/cekura-ai-dashboards-api-openapi.yml
- filename: cekura-ai-evaluators-api-openapi.yml
  format: yaml
  label: Cekura Evaluators API
  slug: cekura-ai-evaluators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cekura-ai/openapi/cekura-ai-evaluators-api-openapi.yml
- filename: cekura-ai-metrics-api-openapi.yml
  format: yaml
  label: Cekura Metrics API
  slug: cekura-ai-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cekura-ai/openapi/cekura-ai-metrics-api-openapi.yml
- filename: cekura-ai-observability-api-openapi.yml
  format: yaml
  label: Cekura Observability API
  slug: cekura-ai-observability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cekura-ai/openapi/cekura-ai-observability-api-openapi.yml
- filename: cekura-ai-results-api-openapi.yml
  format: yaml
  label: Cekura Results API
  slug: cekura-ai-results-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cekura-ai/openapi/cekura-ai-results-api-openapi.yml
- filename: cekura-ai-runs-api-openapi.yml
  format: yaml
  label: Cekura Runs API
  slug: cekura-ai-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cekura-ai/openapi/cekura-ai-runs-api-openapi.yml
- filename: cekura-ai-scenarios-api-openapi.yml
  format: yaml
  label: Cekura Scenarios API
  slug: cekura-ai-scenarios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cekura-ai/openapi/cekura-ai-scenarios-api-openapi.yml
- filename: cekura-ai-schedules-api-openapi.yml
  format: yaml
  label: Cekura Schedules API
  slug: cekura-ai-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cekura-ai/openapi/cekura-ai-schedules-api-openapi.yml
- filename: cekura-ai-slack-api-openapi.yml
  format: yaml
  label: Cekura Slack API
  slug: cekura-ai-slack-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cekura-ai/openapi/cekura-ai-slack-api-openapi.yml
- filename: cekura-ai-test-framework-api-openapi.yml
  format: yaml
  label: Cekura Test Framework API
  slug: cekura-ai-test-framework-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cekura-ai/openapi/cekura-ai-test-framework-api-openapi.yml
- filename: cekura-ai-user-api-openapi.yml
  format: yaml
  label: Cekura User API
  slug: cekura-ai-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cekura-ai/openapi/cekura-ai-user-api-openapi.yml
auth_types: []
description: Authentication methods published for Cekura API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cekura Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cekura declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cekura
provider_slug: cekura-ai
scheme_count: 2
schemes:
- evidence: API Key Authentication. It should be included in the header of each request.
  header: X-CEKURA-API-KEY
  how_to_obtain: Create a new API key via the /user/api/v1/user-api-key/ endpoint.
  location: header
  name: api_key
  type: apiKey
- evidence: Cekura dashboard session token. Not a customer API credential.
  header: Authorization
  how_to_obtain: Obtain a session token from the Cekura dashboard after logging in.
  location: header
  name: supabase_session
  type: http-bearer
slug: cekura-ai-authentication
source_filename: cekura-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.cekura.ai/api-reference/user/create-api-key.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.cekura.ai/api-reference/user/create-api-key.md\nsources:\n- https://docs.cekura.ai/api-reference/user/create-api-key.md\n- https://docs.cekura.ai/documentation/embed/generate-token.md\n- https://docs.cekura.ai/documentation/embed/refreshing-expired-token.md\n- https://docs.cekura.ai/documentation/key-concepts/agents/Agent_Setup_Guide.md\ndescription: Authentication methods published for Cekura API\nschemes:\n- type: apiKey\n  name: api_key\n  evidence: API Key Authentication. It should be included in the header of each request.\n  location: header\n  header: X-CEKURA-API-KEY\n  how_to_obtain: Create a new API key via the /user/api/v1/user-api-key/ endpoint.\n- type: http-bearer\n  name: supabase_session\n  evidence: Cekura dashboard session token. Not a customer API credential.\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a session token from\
  \ the Cekura dashboard after logging in.\ndocs: https://docs.cekura.ai/api-reference/user/create-api-key.md\n"
source_yaml_url: https://artifacts.apis.io/cekura-ai/authentication/cekura-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- VoiceAI
- QA
- Testing
- Benchmarking
---
