---
anonymous_access: false
api_key_in: []
api_specs:
- filename: oruk-ai-affect-api-openapi.yml
  format: yaml
  label: oruk-ai Affect API
  slug: oruk-ai-affect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-affect-api-openapi.yml
- filename: oruk-ai-audio-api-openapi.yml
  format: yaml
  label: oruk-ai Audio API
  slug: oruk-ai-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-audio-api-openapi.yml
- filename: oruk-ai-client-token-api-openapi.yml
  format: yaml
  label: oruk-ai Client Token API
  slug: oruk-ai-client-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-client-token-api-openapi.yml
- filename: oruk-ai-livez-api-openapi.yml
  format: yaml
  label: oruk-ai Livez API
  slug: oruk-ai-livez-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-livez-api-openapi.yml
- filename: oruk-ai-models-api-openapi.yml
  format: yaml
  label: oruk-ai Models API
  slug: oruk-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-models-api-openapi.yml
- filename: oruk-ai-orukzero-api-openapi.yml
  format: yaml
  label: oruk-ai Oruk Zero API
  slug: oruk-ai-orukzero-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-orukzero-api-openapi.yml
- filename: oruk-ai-pricing-api-openapi.yml
  format: yaml
  label: oruk-ai Pricing API
  slug: oruk-ai-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-pricing-api-openapi.yml
- filename: oruk-ai-readyz-api-openapi.yml
  format: yaml
  label: oruk-ai Readyz API
  slug: oruk-ai-readyz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-readyz-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Oruk Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: oruk-ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: oruk-ai
provider_slug: oruk-ai
scheme_count: 1
schemes:
- bearerFormat: oruk API key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/oruk-ai.json
  type: http
slug: oruk-ai-authentication
source_filename: oruk-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/oruk-ai.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: oruk API key\n  sources:\n  - openapi/oruk-ai.json\n"
source_yaml_url: https://artifacts.apis.io/oruk-ai/authentication/oruk-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Speech
- AI
- Transcription
- Voice
---
