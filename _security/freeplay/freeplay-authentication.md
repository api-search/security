---
anonymous_access: false
api_key_in: []
api_specs:
- filename: freeplay-agents-api-openapi.yml
  format: yaml
  label: Freeplay Agents API
  slug: freeplay-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-agents-api-openapi.yml
- filename: freeplay-prompt-templates-api-openapi.yml
  format: yaml
  label: Freeplay Prompt Templates API
  slug: freeplay-prompt-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-prompt-templates-api-openapi.yml
- filename: freeplay-test-runs-api-openapi.yml
  format: yaml
  label: Freeplay Test Runs API
  slug: freeplay-test-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-test-runs-api-openapi.yml
- filename: freeplay-agent-datasets-api-openapi.yml
  format: yaml
  label: Freeplay Agent Datasets API
  slug: freeplay-agent-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-agent-datasets-api-openapi.yml
- filename: freeplay-configuration-api-openapi.yml
  format: yaml
  label: Freeplay Configuration API
  slug: freeplay-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-configuration-api-openapi.yml
- filename: freeplay-evaluation-criteria-api-openapi.yml
  format: yaml
  label: Freeplay Evaluation Criteria API
  slug: freeplay-evaluation-criteria-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-evaluation-criteria-api-openapi.yml
- filename: freeplay-insights-api-openapi.yml
  format: yaml
  label: Freeplay Insights API
  slug: freeplay-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-insights-api-openapi.yml
- filename: freeplay-models-api-openapi.yml
  format: yaml
  label: Freeplay Models API
  slug: freeplay-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-models-api-openapi.yml
- filename: freeplay-observability-api-openapi.yml
  format: yaml
  label: Freeplay Observability API
  slug: freeplay-observability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-observability-api-openapi.yml
- filename: freeplay-prompt-datasets-api-openapi.yml
  format: yaml
  label: Freeplay Prompt Datasets API
  slug: freeplay-prompt-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-prompt-datasets-api-openapi.yml
- filename: freeplay-prompt-optimization-api-openapi.yml
  format: yaml
  label: Freeplay Prompt Optimization API
  slug: freeplay-prompt-optimization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-prompt-optimization-api-openapi.yml
- filename: freeplay-review-queues-api-openapi.yml
  format: yaml
  label: Freeplay Review Queues API
  slug: freeplay-review-queues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-review-queues-api-openapi.yml
- filename: freeplay-saved-searches-api-openapi.yml
  format: yaml
  label: Freeplay Saved Searches API
  slug: freeplay-saved-searches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-saved-searches-api-openapi.yml
- filename: freeplay-search-analytics-api-openapi.yml
  format: yaml
  label: Freeplay Search & Analytics API
  slug: freeplay-search-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-search-analytics-api-openapi.yml
- filename: freeplay-tags-api-openapi.yml
  format: yaml
  label: Freeplay Tags API
  slug: freeplay-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-tags-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Freeplay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Freeplay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Freeplay
provider_slug: freeplay
scheme_count: 1
schemes:
- description: Authenticate requests using your Freeplay API key as a Bearer token in the Authorization header. API keys are managed at https://app.freeplay.ai/settings/api-access.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/freeplay-openapi.yml
  type: http
slug: freeplay-authentication
source_filename: freeplay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/freeplay-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Authenticate requests using your Freeplay API key as a Bearer token in the Authorization\n    header. API keys are managed at https://app.freeplay.ai/settings/api-access.\n  sources:\n  - openapi/freeplay-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/freeplay/authentication/freeplay-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- LLM
- Evaluation
- Observability
- Prompt Management
- Experimentation
---
