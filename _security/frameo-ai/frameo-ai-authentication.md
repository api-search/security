---
anonymous_access: false
api_key_in: []
api_specs:
- filename: frameo-ai-account-api-openapi.yml
  format: yaml
  label: Frameo Account API
  slug: frameo-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frameo-ai/openapi/frameo-ai-account-api-openapi.yml
- filename: frameo-ai-events-api-openapi.yml
  format: yaml
  label: Frameo Events API
  slug: frameo-ai-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frameo-ai/openapi/frameo-ai-events-api-openapi.yml
- filename: frameo-ai-generations-api-openapi.yml
  format: yaml
  label: Frameo Generations API
  slug: frameo-ai-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frameo-ai/openapi/frameo-ai-generations-api-openapi.yml
- filename: frameo-ai-models-api-openapi.yml
  format: yaml
  label: Frameo Models API
  slug: frameo-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frameo-ai/openapi/frameo-ai-models-api-openapi.yml
- filename: frameo-ai-uploads-api-openapi.yml
  format: yaml
  label: Frameo Uploads API
  slug: frameo-ai-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frameo-ai/openapi/frameo-ai-uploads-api-openapi.yml
- filename: frameo-ai-webhooks-api-openapi.yml
  format: yaml
  label: Frameo Webhooks API
  slug: frameo-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frameo-ai/openapi/frameo-ai-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Frameo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Frameo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Frameo
provider_slug: frameo-ai
scheme_count: 1
schemes:
- description: Your API key, fk_live_...
  name: apiKey
  scheme: bearer
  sources:
  - openapi/frameo-ai-openapi.json
  type: http
slug: frameo-ai-authentication
source_filename: frameo-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/frameo-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: Your API key, fk_live_...\n  sources:\n  - openapi/frameo-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/frameo-ai/authentication/frameo-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Video
- Production
- Platform
- Creative
---
