---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: hedra-access-api-openapi.yml
  format: yaml
  label: Hedra Access API
  slug: hedra-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedra/openapi/hedra-access-api-openapi.yml
- filename: hedra-billing-api-openapi.yml
  format: yaml
  label: Hedra Billing API
  slug: hedra-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedra/openapi/hedra-billing-api-openapi.yml
- filename: hedra-jobs-api-openapi.yml
  format: yaml
  label: Hedra Jobs API
  slug: hedra-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedra/openapi/hedra-jobs-api-openapi.yml
- filename: hedra-log-drains-api-openapi.yml
  format: yaml
  label: Hedra Log drains API
  slug: hedra-log-drains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedra/openapi/hedra-log-drains-api-openapi.yml
- filename: hedra-models-api-openapi.yml
  format: yaml
  label: Hedra Models API
  slug: hedra-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedra/openapi/hedra-models-api-openapi.yml
- filename: hedra-run-a-model-api-openapi.yml
  format: yaml
  label: Hedra Run a model API
  slug: hedra-run-a-model-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedra/openapi/hedra-run-a-model-api-openapi.yml
- filename: hedra-webhooks-api-openapi.yml
  format: yaml
  label: Hedra Webhooks API
  slug: hedra-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedra/openapi/hedra-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Hedra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hedra secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hedra
provider_slug: hedra
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/hedra-web-api-openapi-original.json
  type: apiKey
slug: hedra-authentication
source_filename: hedra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/hedra-web-api-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/hedra-web-api-openapi-original.json\n"
source_yaml_url: https://artifacts.apis.io/hedra/authentication/hedra-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Generative AI
- Video Generation
- Image Generation
- Audio Generation
- Text-to-Speech
- Avatars
- Media
- Machine Learning
---
