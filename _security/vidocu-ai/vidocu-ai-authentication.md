---
anonymous_access: false
api_key_in: []
api_specs:
- filename: vidocu-ai-ai-recorder-api-openapi.yml
  format: yaml
  label: vidocu-ai AI Recorder API
  slug: vidocu-ai-ai-recorder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-ai-recorder-api-openapi.yml
- filename: vidocu-ai-brand-kit-api-openapi.yml
  format: yaml
  label: vidocu-ai Brand Kit API
  slug: vidocu-ai-brand-kit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-brand-kit-api-openapi.yml
- filename: vidocu-ai-courses-api-openapi.yml
  format: yaml
  label: vidocu-ai Courses API
  slug: vidocu-ai-courses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-courses-api-openapi.yml
- filename: vidocu-ai-governance-api-openapi.yml
  format: yaml
  label: vidocu-ai Governance API
  slug: vidocu-ai-governance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-governance-api-openapi.yml
- filename: vidocu-ai-jobs-api-openapi.yml
  format: yaml
  label: vidocu-ai Jobs API
  slug: vidocu-ai-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-jobs-api-openapi.yml
- filename: vidocu-ai-knowledge-center-api-openapi.yml
  format: yaml
  label: vidocu-ai Knowledge Center API
  slug: vidocu-ai-knowledge-center-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-knowledge-center-api-openapi.yml
- filename: vidocu-ai-operations-api-openapi.yml
  format: yaml
  label: vidocu-ai Operations API
  slug: vidocu-ai-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-operations-api-openapi.yml
- filename: vidocu-ai-projects-api-openapi.yml
  format: yaml
  label: vidocu-ai Projects API
  slug: vidocu-ai-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-projects-api-openapi.yml
- filename: vidocu-ai-reference-api-openapi.yml
  format: yaml
  label: vidocu-ai Reference API
  slug: vidocu-ai-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-reference-api-openapi.yml
- filename: vidocu-ai-remix-api-openapi.yml
  format: yaml
  label: vidocu-ai Remix API
  slug: vidocu-ai-remix-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-remix-api-openapi.yml
- filename: vidocu-ai-studio-api-openapi.yml
  format: yaml
  label: vidocu-ai Studio API
  slug: vidocu-ai-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-studio-api-openapi.yml
- filename: vidocu-ai-tools-api-openapi.yml
  format: yaml
  label: vidocu-ai Tools API
  slug: vidocu-ai-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-tools-api-openapi.yml
- filename: vidocu-ai-training-modules-api-openapi.yml
  format: yaml
  label: vidocu-ai Training Modules API
  slug: vidocu-ai-training-modules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-training-modules-api-openapi.yml
- filename: vidocu-ai-usage-api-openapi.yml
  format: yaml
  label: vidocu-ai Usage API
  slug: vidocu-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-usage-api-openapi.yml
- filename: vidocu-ai-videos-api-openapi.yml
  format: yaml
  label: vidocu-ai Videos API
  slug: vidocu-ai-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-videos-api-openapi.yml
- filename: vidocu-ai-webhooks-api-openapi.yml
  format: yaml
  label: vidocu-ai Webhooks API
  slug: vidocu-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Vidocu Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: vidocu-ai secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: vidocu-ai
provider_slug: vidocu-ai
scheme_count: 2
schemes:
- description: An API key (`vdo_live_...`) or an OAuth 2.0 access token (`vdo_oat_...`).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/support-vidocu-openapi.json
  - openapi/vidocu-ai-openapi.json
  type: http
- flows:
  - authorizationUrl: https://vidocu.ai/oauth/authorize
    flow: authorizationCode
    scopes: 42
    tokenUrl: https://api.vidocu.ai/oauth/token
  name: oauth2
  sources:
  - openapi/support-vidocu-openapi.json
  - openapi/vidocu-ai-openapi.json
  type: oauth2
slug: vidocu-ai-authentication
source_filename: vidocu-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/support-vidocu-openapi.json, openapi/vidocu-ai-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: An API key (`vdo_live_...`) or an OAuth 2.0 access token (`vdo_oat_...`).\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://vidocu.ai/oauth/authorize\n    tokenUrl: https://api.vidocu.ai/oauth/token\n    scopes: 42\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/vidocu-ai/authentication/vidocu-ai-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Artificial Intelligence
- Video
- Documentation
- SOP
- Training
- Knowledge Base
---
