---
anonymous_access: false
api_key_in: []
api_specs:
- filename: api-stock-com-account-management-api-openapi.yml
  format: yaml
  label: api-stock-com Account Management API
  slug: api-stock-com-account-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-stock-com/openapi/api-stock-com-account-management-api-openapi.yml
- filename: api-stock-com-agent-api-openapi.yml
  format: yaml
  label: api-stock-com Agent API
  slug: api-stock-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-stock-com/openapi/api-stock-com-agent-api-openapi.yml
- filename: api-stock-com-catalog-api-openapi.yml
  format: yaml
  label: api-stock-com Catalog API
  slug: api-stock-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-stock-com/openapi/api-stock-com-catalog-api-openapi.yml
- filename: api-stock-com-costs-api-openapi.yml
  format: yaml
  label: api-stock-com Costs API
  slug: api-stock-com-costs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-stock-com/openapi/api-stock-com-costs-api-openapi.yml
- filename: api-stock-com-generations-api-openapi.yml
  format: yaml
  label: api-stock-com Generations API
  slug: api-stock-com-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-stock-com/openapi/api-stock-com-generations-api-openapi.yml
- filename: api-stock-com-llm-api-openapi.yml
  format: yaml
  label: api-stock-com LLM API
  slug: api-stock-com-llm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-stock-com/openapi/api-stock-com-llm-api-openapi.yml
- filename: api-stock-com-task-management-api-openapi.yml
  format: yaml
  label: api-stock-com Task Management API
  slug: api-stock-com-task-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-stock-com/openapi/api-stock-com-task-management-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Api Stock Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: api-stock-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: api-stock-com
provider_slug: api-stock-com
scheme_count: 2
schemes:
- description: Bearer <your API key>
  in: header
  name: Authorization
  type: apiKey
- description: API key header alternative
  in: header
  name: x-api-key
  type: apiKey
slug: api-stock-com-authentication
source_filename: api-stock-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: https://docs.api-stock.com/docs/authentication\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Bearer <your API key>\"\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: \"API key header alternative\"\n"
source_yaml_url: https://artifacts.apis.io/api-stock-com/authentication/api-stock-com-authentication.yml
summary_line: 2 schemes
tags:
- AI
- Machine Learning
- LLM
- API
- Platform
---
