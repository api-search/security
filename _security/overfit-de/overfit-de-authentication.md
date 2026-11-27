---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: overfit-de-agent-interaction-api-openapi.yml
  format: yaml
  label: Overfit Agent Interaction API
  slug: overfit-de-agent-interaction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overfit-de/openapi/overfit-de-agent-interaction-api-openapi.yml
- filename: overfit-de-agents-api-openapi.yml
  format: yaml
  label: Overfit Agents API
  slug: overfit-de-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overfit-de/openapi/overfit-de-agents-api-openapi.yml
- filename: overfit-de-aithra-api-openapi.yml
  format: yaml
  label: Overfit Aithra API
  slug: overfit-de-aithra-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overfit-de/openapi/overfit-de-aithra-api-openapi.yml
- filename: overfit-de-conversations-api-openapi.yml
  format: yaml
  label: Overfit Conversations API
  slug: overfit-de-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overfit-de/openapi/overfit-de-conversations-api-openapi.yml
- filename: overfit-de-feedback-api-openapi.yml
  format: yaml
  label: Overfit Feedback API
  slug: overfit-de-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overfit-de/openapi/overfit-de-feedback-api-openapi.yml
- filename: overfit-de-graph-configs-api-openapi.yml
  format: yaml
  label: Overfit Graph Configs API
  slug: overfit-de-graph-configs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overfit-de/openapi/overfit-de-graph-configs-api-openapi.yml
- filename: overfit-de-graphs-api-openapi.yml
  format: yaml
  label: Overfit Graphs API
  slug: overfit-de-graphs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overfit-de/openapi/overfit-de-graphs-api-openapi.yml
- filename: overfit-de-insights-api-openapi.yml
  format: yaml
  label: Overfit Insights API
  slug: overfit-de-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overfit-de/openapi/overfit-de-insights-api-openapi.yml
- filename: overfit-de-letter-v2-api-openapi.yml
  format: yaml
  label: Overfit Letter V2 API
  slug: overfit-de-letter-v2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overfit-de/openapi/overfit-de-letter-v2-api-openapi.yml
- filename: overfit-de-models-api-openapi.yml
  format: yaml
  label: Overfit Models API
  slug: overfit-de-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overfit-de/openapi/overfit-de-models-api-openapi.yml
- filename: overfit-de-questions-api-openapi.yml
  format: yaml
  label: Overfit Questions API
  slug: overfit-de-questions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overfit-de/openapi/overfit-de-questions-api-openapi.yml
- filename: overfit-de-sources-api-openapi.yml
  format: yaml
  label: Overfit Sources API
  slug: overfit-de-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overfit-de/openapi/overfit-de-sources-api-openapi.yml
- filename: overfit-de-system-api-openapi.yml
  format: yaml
  label: Overfit System API
  slug: overfit-de-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overfit-de/openapi/overfit-de-system-api-openapi.yml
- filename: overfit-de-tools-api-openapi.yml
  format: yaml
  label: Overfit Tools API
  slug: overfit-de-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overfit-de/openapi/overfit-de-tools-api-openapi.yml
auth_types:
- apiKey
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Overfit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Overfit secures its APIs with apiKey and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Overfit
provider_slug: overfit-de
scheme_count: 2
schemes:
- name: OpenIdConnect
  openIdConnectUrl: https://auth.okns.de/realms/overfit-products/.well-known/openid-configuration
  sources:
  - openapi/overfit-de-openapi.json
  type: openIdConnect
- in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/overfit-de-openapi.json
  type: apiKey
slug: overfit-de-authentication
source_filename: overfit-de-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/overfit-de-openapi.json\nsummary:\n  types:\n  - apiKey\n  - openIdConnect\n  api_key_in:\n  - header\nschemes:\n- name: OpenIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.okns.de/realms/overfit-products/.well-known/openid-configuration\n  sources:\n  - openapi/overfit-de-openapi.json\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/overfit-de-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/overfit-de/authentication/overfit-de-authentication.yml
summary_line: apiKey/openIdConnect · 2 schemes
tags:
- Artificial Intelligence
- Edge Computing
- Industrial Automation
- Data Sovereignty
- German
---
