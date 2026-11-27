---
anonymous_access: false
api_key_in: []
api_specs:
- filename: memoryplugin-com-buckets-api-openapi.yml
  format: yaml
  label: MemoryPlugin Buckets API
  slug: memoryplugin-com-buckets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memoryplugin-com/openapi/memoryplugin-com-buckets-api-openapi.yml
- filename: memoryplugin-com-chat-history-api-openapi.yml
  format: yaml
  label: MemoryPlugin Chat History API
  slug: memoryplugin-com-chat-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memoryplugin-com/openapi/memoryplugin-com-chat-history-api-openapi.yml
- filename: memoryplugin-com-memories-api-openapi.yml
  format: yaml
  label: MemoryPlugin Memories API
  slug: memoryplugin-com-memories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memoryplugin-com/openapi/memoryplugin-com-memories-api-openapi.yml
- filename: memoryplugin-com-memory-api-openapi.yml
  format: yaml
  label: MemoryPlugin Memory API
  slug: memoryplugin-com-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memoryplugin-com/openapi/memoryplugin-com-memory-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: MemoryPlugin Authentication
name_suffix: Authentication
oauth_flows: []
overview: MemoryPlugin secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MemoryPlugin
provider_slug: memoryplugin-com
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/memoryplugin-com-openapi.json
  type: http
slug: memoryplugin-com-authentication
source_filename: memoryplugin-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/memoryplugin-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/memoryplugin-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/memoryplugin-com/authentication/memoryplugin-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Memory
- Integration
- Software-as-a-Service
- Productivity
---
