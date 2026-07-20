---
api_key_in:
- header
api_specs:
- filename: coval-agents-openapi.yml
  format: yaml
  label: Coval API
  slug: coval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval/refs/heads/main/openapi/coval-agents-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Coval Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coval secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Coval
provider_slug: coval
scheme_count: 2
schemes:
- description: API key for authentication
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/coval-agents-openapi.yml
  - openapi/coval-organization-openapi.yml
  - openapi/coval-reports-openapi.yml
  type: apiKey
- description: API key for authentication
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/coval-api-keys-openapi.yml
  - openapi/coval-conversations-openapi.yml
  - openapi/coval-dashboards-openapi.yml
  - openapi/coval-metrics-openapi.yml
  - openapi/coval-monitors-openapi.yml
  - openapi/coval-mutations-openapi.yml
  - openapi/coval-personas-openapi.yml
  - openapi/coval-reviews-openapi.yml
  - openapi/coval-run-templates-openapi.yml
  - openapi/coval-runs-openapi.yml
  - openapi/coval-scheduled-runs-openapi.yml
  - openapi/coval-simulations-openapi.yml
  - openapi/coval-tags-openapi.yml
  - openapi/coval-test-cases-openapi.yml
  - openapi/coval-test-sets-openapi.yml
  - openapi/coval-traces-openapi.yml
  - openapi/coval-webhooks-openapi.yml
  type: apiKey
slug: coval-authentication
source_filename: coval-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\ndocs: https://docs.coval.ai/api-reference/v1/introduction\nnote: >-\n  Single scheme: an organization API key sent in the X-API-Key request header on every call.\n  Keys are issued/rotated from the dashboard (https://app.coval.dev/settings) and managed via the\n  api-keys API. No OAuth/OIDC — scopes/ intentionally omitted.\nsource: openapi/coval-agents-openapi.yml, openapi/coval-api-keys-openapi.yml, openapi/coval-conversations-openapi.yml,\n  openapi/coval-dashboards-openapi.yml, openapi/coval-metrics-openapi.yml, openapi/coval-monitors-openapi.yml,\n  openapi/coval-mutations-openapi.yml, openapi/coval-organization-openapi.yml, openapi/coval-personas-openapi.yml,\n  openapi/coval-reports-openapi.yml, openapi/coval-reviews-openapi.yml, openapi/coval-run-templates-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description:\
  \ API key for authentication\n  sources:\n  - openapi/coval-agents-openapi.yml\n  - openapi/coval-organization-openapi.yml\n  - openapi/coval-reports-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key for authentication\n  sources:\n  - openapi/coval-api-keys-openapi.yml\n  - openapi/coval-conversations-openapi.yml\n  - openapi/coval-dashboards-openapi.yml\n  - openapi/coval-metrics-openapi.yml\n  - openapi/coval-monitors-openapi.yml\n  - openapi/coval-mutations-openapi.yml\n  - openapi/coval-personas-openapi.yml\n  - openapi/coval-reviews-openapi.yml\n  - openapi/coval-run-templates-openapi.yml\n  - openapi/coval-runs-openapi.yml\n  - openapi/coval-scheduled-runs-openapi.yml\n  - openapi/coval-simulations-openapi.yml\n  - openapi/coval-tags-openapi.yml\n  - openapi/coval-test-cases-openapi.yml\n  - openapi/coval-test-sets-openapi.yml\n  - openapi/coval-traces-openapi.yml\n  - openapi/coval-webhooks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coval/refs/heads/main/authentication/coval-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- AI Agents
- Voice AI
- Testing
- Evaluation
- Simulation
- Observability
- Conversational AI
- LLM
- Quality Assurance
---
