---
api_key_in:
- header
api_specs:
- filename: aito-technologies-openapi-original.yml
  format: yaml
  label: Aito.ai Query API
  slug: aitoai-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aito-technologies/refs/heads/main/openapi/aito-technologies-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Aito Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aito Technologies secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aito Technologies
provider_slug: aito-technologies
scheme_count: 1
schemes:
- docs: https://aito.ai/docs/api/
  in: header
  key_types:
  - read-only
  - read/write
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/aito-technologies-openapi-original.yml
  type: apiKey
slug: aito-technologies-authentication
source_filename: aito-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/aito-technologies-openapi-original.yml\ndocs: https://aito.ai/docs/api/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  key_types:\n  - read-only\n  - read/write\n  env_vars:\n  - AITO_INSTANCE_URL\n  - AITO_API_KEY\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  key_types:\n  - read-only\n  - read/write\n  docs: https://aito.ai/docs/api/\n  sources:\n  - openapi/aito-technologies-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aito-technologies/refs/heads/main/authentication/aito-technologies-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Predictive Database
- Machine Learning
- Artificial Intelligence
- Recommendations
- Search
- Predictive Analytics
- Automation
- Data
---
