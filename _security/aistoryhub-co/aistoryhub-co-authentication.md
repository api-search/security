---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aistoryhub-co-account-api-openapi.yml
  format: yaml
  label: AIStoryHub Account API
  slug: aistoryhub-co-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aistoryhub-co/openapi/aistoryhub-co-account-api-openapi.yml
- filename: aistoryhub-co-ai-api-openapi.yml
  format: yaml
  label: AIStoryHub AI API
  slug: aistoryhub-co-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aistoryhub-co/openapi/aistoryhub-co-ai-api-openapi.yml
- filename: aistoryhub-co-chapters-api-openapi.yml
  format: yaml
  label: AIStoryHub Chapters API
  slug: aistoryhub-co-chapters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aistoryhub-co/openapi/aistoryhub-co-chapters-api-openapi.yml
- filename: aistoryhub-co-memory-api-openapi.yml
  format: yaml
  label: AIStoryHub Memory API
  slug: aistoryhub-co-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aistoryhub-co/openapi/aistoryhub-co-memory-api-openapi.yml
- filename: aistoryhub-co-rules-api-openapi.yml
  format: yaml
  label: AIStoryHub Rules API
  slug: aistoryhub-co-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aistoryhub-co/openapi/aistoryhub-co-rules-api-openapi.yml
- filename: aistoryhub-co-skills-api-openapi.yml
  format: yaml
  label: AIStoryHub Skills API
  slug: aistoryhub-co-skills-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aistoryhub-co/openapi/aistoryhub-co-skills-api-openapi.yml
- filename: aistoryhub-co-stories-api-openapi.yml
  format: yaml
  label: AIStoryHub Stories API
  slug: aistoryhub-co-stories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aistoryhub-co/openapi/aistoryhub-co-stories-api-openapi.yml
- filename: aistoryhub-co-voice-api-openapi.yml
  format: yaml
  label: AIStoryHub Voice API
  slug: aistoryhub-co-voice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aistoryhub-co/openapi/aistoryhub-co-voice-api-openapi.yml
- filename: aistoryhub-co-world-api-openapi.yml
  format: yaml
  label: AIStoryHub World API
  slug: aistoryhub-co-world-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aistoryhub-co/openapi/aistoryhub-co-world-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: AIStoryHub Authentication
name_suffix: Authentication
oauth_flows: []
overview: AIStoryHub secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AIStoryHub
provider_slug: aistoryhub-co
scheme_count: 1
schemes:
- bearerFormat: ash_...
  description: 'Create a token under Settings, Developer API and send it as `Authorization: Bearer ash_...`. Each endpoint requires one scope, listed per-operation via the `x-required-scope` extension; see https://aistoryhub.co/developers for the full scope list.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/aistoryhub-co-openapi.json
  type: http
slug: aistoryhub-co-authentication
source_filename: aistoryhub-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/aistoryhub-co-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: ash_...\n  description: 'Create a token under Settings, Developer API and send it as `Authorization:\n    Bearer ash_...`. Each endpoint requires one scope, listed per-operation via the `x-required-scope`\n    extension; see https://aistoryhub.co/developers for the full scope list.'\n  sources:\n  - openapi/aistoryhub-co-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/aistoryhub-co/authentication/aistoryhub-co-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Writing
- Fiction
- Platform
- Free
---
