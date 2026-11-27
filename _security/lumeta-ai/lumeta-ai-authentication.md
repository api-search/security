---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lumeta-ai-account-api-openapi.yml
  format: yaml
  label: Lumeta AI Account API
  slug: lumeta-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumeta-ai/openapi/lumeta-ai-account-api-openapi.yml
- filename: lumeta-ai-estimate-api-openapi.yml
  format: yaml
  label: Lumeta AI Estimate API
  slug: lumeta-ai-estimate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumeta-ai/openapi/lumeta-ai-estimate-api-openapi.yml
- filename: lumeta-ai-files-api-openapi.yml
  format: yaml
  label: Lumeta AI Files API
  slug: lumeta-ai-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumeta-ai/openapi/lumeta-ai-files-api-openapi.yml
- filename: lumeta-ai-generations-api-openapi.yml
  format: yaml
  label: Lumeta AI Generations API
  slug: lumeta-ai-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumeta-ai/openapi/lumeta-ai-generations-api-openapi.yml
- filename: lumeta-ai-lumeta-api-api-openapi.yml
  format: yaml
  label: Lumeta AI Lumeta API
  slug: lumeta-ai-lumeta-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumeta-ai/openapi/lumeta-ai-lumeta-api-api-openapi.yml
- filename: lumeta-ai-models-api-openapi.yml
  format: yaml
  label: Lumeta AI Models API
  slug: lumeta-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumeta-ai/openapi/lumeta-ai-models-api-openapi.yml
- filename: lumeta-ai-openapi-json-api-openapi.yml
  format: yaml
  label: Lumeta AI Openapi.json API
  slug: lumeta-ai-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumeta-ai/openapi/lumeta-ai-openapi-json-api-openapi.yml
- filename: lumeta-ai-projects-api-openapi.yml
  format: yaml
  label: Lumeta AI Projects API
  slug: lumeta-ai-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumeta-ai/openapi/lumeta-ai-projects-api-openapi.yml
- filename: lumeta-ai-shelves-api-openapi.yml
  format: yaml
  label: Lumeta AI Shelves API
  slug: lumeta-ai-shelves-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumeta-ai/openapi/lumeta-ai-shelves-api-openapi.yml
- filename: lumeta-ai-teams-api-openapi.yml
  format: yaml
  label: Lumeta AI Teams API
  slug: lumeta-ai-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumeta-ai/openapi/lumeta-ai-teams-api-openapi.yml
- filename: lumeta-ai-voices-api-openapi.yml
  format: yaml
  label: Lumeta AI Voices API
  slug: lumeta-ai-voices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumeta-ai/openapi/lumeta-ai-voices-api-openapi.yml
- filename: lumeta-ai-webhook-endpoints-api-openapi.yml
  format: yaml
  label: Lumeta AI Webhook Endpoints API
  slug: lumeta-ai-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumeta-ai/openapi/lumeta-ai-webhook-endpoints-api-openapi.yml
- filename: lumeta-ai-well-known-api-openapi.yml
  format: yaml
  label: Lumeta AI .well Known API
  slug: lumeta-ai-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumeta-ai/openapi/lumeta-ai-well-known-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Lumeta AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lumeta AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lumeta AI
provider_slug: lumeta-ai
scheme_count: 1
schemes:
- description: 'A personal API key (lm_live_...) or an OAuth access token (lma_...). Scopes: read, generate, library, share (add and remove people on projects and teams, team invites, asking a team''s admins and answering as one).'
  name: bearer
  scheme: bearer
  sources:
  - openapi/lumeta-ai-openapi.json
  type: http
slug: lumeta-ai-authentication
source_filename: lumeta-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/lumeta-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: 'A personal API key (lm_live_...) or an OAuth access token (lma_...). Scopes:\n    read, generate, library, share (add and remove people on projects and teams, team invites,\n    asking a team''s admins and answering as one).'\n  sources:\n  - openapi/lumeta-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/lumeta-ai/authentication/lumeta-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Generative AI
- Image
- Video
- Audio
- Platform
---
