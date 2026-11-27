---
anonymous_access: false
api_key_in: []
api_specs:
- filename: compoid-com-completions-api-openapi.yml
  format: yaml
  label: Compoid Completions API
  slug: compoid-com-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-completions-api-openapi.yml
- filename: compoid-com-detokenize-api-openapi.yml
  format: yaml
  label: Compoid Detokenize API
  slug: compoid-com-detokenize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-detokenize-api-openapi.yml
- filename: compoid-com-generative-scoring-api-openapi.yml
  format: yaml
  label: Compoid Generative Scoring API
  slug: compoid-com-generative-scoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-generative-scoring-api-openapi.yml
- filename: compoid-com-health-api-openapi.yml
  format: yaml
  label: Compoid Health API
  slug: compoid-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-health-api-openapi.yml
- filename: compoid-com-invocations-api-openapi.yml
  format: yaml
  label: Compoid Invocations API
  slug: compoid-com-invocations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-invocations-api-openapi.yml
- filename: compoid-com-is-scaling-elastic-ep-api-openapi.yml
  format: yaml
  label: Compoid Is Scaling Elastic Ep API
  slug: compoid-com-is-scaling-elastic-ep-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-is-scaling-elastic-ep-api-openapi.yml
- filename: compoid-com-kv-event-sources-api-openapi.yml
  format: yaml
  label: Compoid Kv Event Sources API
  slug: compoid-com-kv-event-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-kv-event-sources-api-openapi.yml
- filename: compoid-com-load-api-openapi.yml
  format: yaml
  label: Compoid Load API
  slug: compoid-com-load-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-load-api-openapi.yml
- filename: compoid-com-messages-api-openapi.yml
  format: yaml
  label: Compoid Messages API
  slug: compoid-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-messages-api-openapi.yml
- filename: compoid-com-metrics-api-openapi.yml
  format: yaml
  label: Compoid Metrics API
  slug: compoid-com-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-metrics-api-openapi.yml
- filename: compoid-com-models-api-openapi.yml
  format: yaml
  label: Compoid Models API
  slug: compoid-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-models-api-openapi.yml
- filename: compoid-com-ping-api-openapi.yml
  format: yaml
  label: Compoid Ping API
  slug: compoid-com-ping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-ping-api-openapi.yml
- filename: compoid-com-responses-api-openapi.yml
  format: yaml
  label: Compoid Responses API
  slug: compoid-com-responses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-responses-api-openapi.yml
- filename: compoid-com-scale-elastic-ep-api-openapi.yml
  format: yaml
  label: Compoid Scale Elastic Ep API
  slug: compoid-com-scale-elastic-ep-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-scale-elastic-ep-api-openapi.yml
- filename: compoid-com-systemone-api-openapi.yml
  format: yaml
  label: Compoid Systemone API
  slug: compoid-com-systemone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-systemone-api-openapi.yml
- filename: compoid-com-tokenize-api-openapi.yml
  format: yaml
  label: Compoid Tokenize API
  slug: compoid-com-tokenize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-tokenize-api-openapi.yml
- filename: compoid-com-version-api-openapi.yml
  format: yaml
  label: Compoid Version API
  slug: compoid-com-version-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-version-api-openapi.yml
- filename: compoid-com-chat-completions-api-openapi.yml
  format: yaml
  label: Compoid Chat Completions API
  slug: compoid-com-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-chat-completions-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Compoid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Compoid declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Compoid
provider_slug: compoid-com
scheme_count: 2
schemes:
- applies_to:
  - https://mcpv.compoid.com/mcp
  - https://www.compoid.com/api
  description: 'Personal repository API token (compoid-<id>) issued to every registered account on the next daily bootstrap sweep. Pass as the X-Compoid-Repo-Key header (or COMPOID_REPO_API_KEY env var for the self-hosted server). Since compoid-mcp 0.1.5, an Authorization: Bearer token is used as the repository key when no X-Compoid-Repo-Key header is present.'
  header: X-Compoid-Repo-Key
  in: header
  name: X-Compoid-Repo-Key
  type: apiKey
- applies_to:
  - https://api.compoid.com/v1
  description: Bearer key the compoid-mcp server sends to the inference API (COMPOID_AI_API_KEY, described in the README as a Pro-subscription key). The provider-hosted OpenAPI declares no securitySchemes.
  name: COMPOID_AI_API_KEY bearer
  scheme: bearer
  source: https://github.com/compoid/compoid-mcp/blob/main/README.md
  type: http
slug: compoid-com-authentication
source_filename: compoid-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.compoid.com/agents.md\ndocs: https://www.compoid.com/documentation\nname: Compoid authentication\nschemes:\n- name: X-Compoid-Repo-Key\n  type: apiKey\n  in: header\n  header: X-Compoid-Repo-Key\n  applies_to: [https://mcpv.compoid.com/mcp, https://www.compoid.com/api]\n  description: 'Personal repository API token (compoid-<id>) issued to every registered account on the next daily bootstrap sweep. Pass as the X-Compoid-Repo-Key header (or COMPOID_REPO_API_KEY env var for the self-hosted server). Since compoid-mcp 0.1.5, an Authorization: Bearer token is used as the repository key when no X-Compoid-Repo-Key header is present.'\n- name: COMPOID_AI_API_KEY bearer\n  type: http\n  scheme: bearer\n  applies_to: [https://api.compoid.com/v1]\n  description: Bearer key the compoid-mcp server sends to the inference API (COMPOID_AI_API_KEY, described in the README as a Pro-subscription key). The provider-hosted OpenAPI declares\
  \ no securitySchemes.\n  source: https://github.com/compoid/compoid-mcp/blob/main/README.md\n"
source_yaml_url: https://artifacts.apis.io/compoid-com/authentication/compoid-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI Agents
- MCP
- Digital Repository
- Research Data
- Datasets
- Knowledge Management
- Agent Memory
---
