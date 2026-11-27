---
anonymous_access: false
api_key_in: []
api_specs:
- filename: crawdar-com-account-api-openapi.yml
  format: yaml
  label: Crawdar Account API
  slug: crawdar-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawdar-com/openapi/crawdar-com-account-api-openapi.yml
- filename: crawdar-com-graph-api-openapi.yml
  format: yaml
  label: Crawdar Graph API
  slug: crawdar-com-graph-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawdar-com/openapi/crawdar-com-graph-api-openapi.yml
- filename: crawdar-com-keys-api-openapi.yml
  format: yaml
  label: Crawdar Keys API
  slug: crawdar-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawdar-com/openapi/crawdar-com-keys-api-openapi.yml
- filename: crawdar-com-learning-api-openapi.yml
  format: yaml
  label: Crawdar Learning API
  slug: crawdar-com-learning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawdar-com/openapi/crawdar-com-learning-api-openapi.yml
- filename: crawdar-com-lists-api-openapi.yml
  format: yaml
  label: Crawdar Lists API
  slug: crawdar-com-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawdar-com/openapi/crawdar-com-lists-api-openapi.yml
- filename: crawdar-com-network-api-openapi.yml
  format: yaml
  label: Crawdar Network API
  slug: crawdar-com-network-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawdar-com/openapi/crawdar-com-network-api-openapi.yml
- filename: crawdar-com-pain-points-api-openapi.yml
  format: yaml
  label: Crawdar Pain Points API
  slug: crawdar-com-pain-points-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawdar-com/openapi/crawdar-com-pain-points-api-openapi.yml
- filename: crawdar-com-quality-benchmark-api-openapi.yml
  format: yaml
  label: Crawdar Quality Benchmark API
  slug: crawdar-com-quality-benchmark-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawdar-com/openapi/crawdar-com-quality-benchmark-api-openapi.yml
- filename: crawdar-com-sandbox-api-openapi.yml
  format: yaml
  label: Crawdar Sandbox API
  slug: crawdar-com-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawdar-com/openapi/crawdar-com-sandbox-api-openapi.yml
- filename: crawdar-com-search-api-openapi.yml
  format: yaml
  label: Crawdar Search API
  slug: crawdar-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawdar-com/openapi/crawdar-com-search-api-openapi.yml
- filename: crawdar-com-searches-api-openapi.yml
  format: yaml
  label: Crawdar Searches API
  slug: crawdar-com-searches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawdar-com/openapi/crawdar-com-searches-api-openapi.yml
- filename: crawdar-com-status-api-openapi.yml
  format: yaml
  label: Crawdar Status API
  slug: crawdar-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawdar-com/openapi/crawdar-com-status-api-openapi.yml
- filename: crawdar-com-workspaces-api-openapi.yml
  format: yaml
  label: Crawdar Workspaces API
  slug: crawdar-com-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawdar-com/openapi/crawdar-com-workspaces-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Crawdar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crawdar declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Crawdar
provider_slug: crawdar-com
scheme_count: 3
schemes:
- description: Account key created while signed in at /account (sign in with ChatGPT); all keys share account limits. The secret is shown once.
  header: x-api-key
  in: header
  name: AgentKey
  type: apiKey
- description: The same account API key may be sent as Authorization Bearer YOUR_KEY.
  name: BearerKey
  scheme: bearer
  type: http
- description: Capability token returned once with a search job; also sent as Authorization Bearer JOB_TOKEN to the job exportUrl.
  header: x-job-token
  in: header
  name: JobToken
  type: apiKey
slug: crawdar-com-authentication
source_filename: crawdar-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://crawdar.com/llms.txt\ndocs: https://crawdar.com/agents\nschemes:\n- name: AgentKey\n  type: apiKey\n  in: header\n  header: x-api-key\n  description: Account key created while signed in at /account (sign in with ChatGPT); all keys share account limits. The secret is shown once.\n- name: BearerKey\n  type: http\n  scheme: bearer\n  description: The same account API key may be sent as Authorization Bearer YOUR_KEY.\n- name: JobToken\n  type: apiKey\n  in: header\n  header: x-job-token\n  description: Capability token returned once with a search job; also sent as Authorization Bearer JOB_TOKEN to the job exportUrl.\nguest_access: Three guest searches in total without a key; sandbox search requires no key.\nkey_management: GET /api/v1/keys reads shared usage and DELETE revokes the presented key; up to two keys can be issued per account per day.\n"
source_yaml_url: https://artifacts.apis.io/crawdar-com/authentication/crawdar-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Business Research
- Lead Generation
- CustomerReviews
- Sales Prospecting
- MCP
- AI Agents
---
