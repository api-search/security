---
anonymous_access: false
api_key_in: []
api_specs:
- filename: topxea-com-anthropic-compatible-api-openapi.yml
  format: yaml
  label: topxea-com Anthropic Compatible API
  slug: topxea-com-anthropic-compatible-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/topxea-com/openapi/topxea-com-anthropic-compatible-api-openapi.yml
- filename: topxea-com-openai-compatible-api-openapi.yml
  format: yaml
  label: topxea-com Open AI Compatible API
  slug: topxea-com-openai-compatible-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/topxea-com/openapi/topxea-com-openai-compatible-api-openapi.yml
- filename: topxea-com-public-api-openapi.yml
  format: yaml
  label: topxea-com Public API
  slug: topxea-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/topxea-com/openapi/topxea-com-public-api-openapi.yml
- filename: topxea-com-typesafe-api-openapi.yml
  format: yaml
  label: topxea-com Type Safe API
  slug: topxea-com-typesafe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/topxea-com/openapi/topxea-com-typesafe-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Topxea Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: topxea-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: topxea-com
provider_slug: topxea-com
scheme_count: 2
schemes:
- description: 'A TopxAI API key (sk-...) as Authorization: Bearer <key>.'
  scheme: bearer
  type: http
- description: The same TopxAI key, the way the Anthropic SDK sends it.
  in: header
  name: x-api-key
  type: apiKey
slug: topxea-com-authentication
source_filename: topxea-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: \"openapi/ai.topxea.com-openapi.json\"\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"A TopxAI API key (sk-...) as Authorization: Bearer <key>.\"\n  - type: apiKey\n    in: header\n    name: x-api-key\n    description: \"The same TopxAI key, the way the Anthropic SDK sends it.\"\n"
source_yaml_url: https://artifacts.apis.io/topxea-com/authentication/topxea-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Data
- Finance
- Research
---
