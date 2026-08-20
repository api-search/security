---
api_key_in: []
api_specs:
- filename: botpress-admin-api-openapi.yml
  format: yaml
  label: Botpress Admin API
  slug: botpress-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botpress/refs/heads/main/openapi/botpress-admin-api-openapi.yml
- filename: botpress-conversations-api-openapi.yml
  format: yaml
  label: Botpress Conversations API
  slug: botpress-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botpress/refs/heads/main/openapi/botpress-conversations-api-openapi.yml
- filename: botpress-files-api-openapi.yml
  format: yaml
  label: Botpress Files API
  slug: botpress-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botpress/refs/heads/main/openapi/botpress-files-api-openapi.yml
- filename: botpress-messages-api-openapi.yml
  format: yaml
  label: Botpress Messages API
  slug: botpress-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botpress/refs/heads/main/openapi/botpress-messages-api-openapi.yml
- filename: botpress-tables-api-openapi.yml
  format: yaml
  label: Botpress Tables API
  slug: botpress-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botpress/refs/heads/main/openapi/botpress-tables-api-openapi.yml
- filename: botpress-users-api-openapi.yml
  format: yaml
  label: Botpress Users API
  slug: botpress-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botpress/refs/heads/main/openapi/botpress-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Botpress Authentication
name_suffix: Authentication
oauth_flows: []
overview: Botpress secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Botpress
provider_slug: botpress
scheme_count: 1
schemes:
- description: Personal access token or workspace API key passed as a Bearer token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/botpress-openapi.yml
  type: http
slug: botpress-authentication
source_filename: botpress-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/botpress-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Personal access token or workspace API key passed as a Bearer token.\n  sources:\n  - openapi/botpress-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/botpress/refs/heads/main/authentication/botpress-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Conversational
- Chat
- Open-Source
- Bot Builder
- LLM
---
