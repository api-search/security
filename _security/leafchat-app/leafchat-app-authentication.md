---
anonymous_access: false
api_key_in: []
api_specs:
- filename: leafchat-app-documents-api-openapi.yml
  format: yaml
  label: leafchat Documents API
  slug: leafchat-app-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leafchat-app/openapi/leafchat-app-documents-api-openapi.yml
- filename: leafchat-app-drafts-api-openapi.yml
  format: yaml
  label: leafchat Drafts API
  slug: leafchat-app-drafts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leafchat-app/openapi/leafchat-app-drafts-api-openapi.yml
- filename: leafchat-app-folders-api-openapi.yml
  format: yaml
  label: leafchat Folders API
  slug: leafchat-app-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leafchat-app/openapi/leafchat-app-folders-api-openapi.yml
- filename: leafchat-app-sources-api-openapi.yml
  format: yaml
  label: leafchat Sources API
  slug: leafchat-app-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leafchat-app/openapi/leafchat-app-sources-api-openapi.yml
- filename: leafchat-app-sync-api-openapi.yml
  format: yaml
  label: leafchat Sync API
  slug: leafchat-app-sync-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leafchat-app/openapi/leafchat-app-sync-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: leafchat Authentication
name_suffix: Authentication
oauth_flows: []
overview: leafchat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: leafchat
provider_slug: leafchat-app
scheme_count: 1
schemes:
- description: ダッシュボードで発行した API キー（lck_ で始まる）
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/leafchat-app-openapi.json
  type: http
slug: leafchat-app-authentication
source_filename: leafchat-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/leafchat-app-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  description: ダッシュボードで発行した API キー（lck_ で始まる）\n  sources:\n  - openapi/leafchat-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/leafchat-app/authentication/leafchat-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Chatbots
- Customer Service
- Automation
- Software-as-a-Service
---
