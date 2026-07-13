---
api_key_in: []
api_specs:
- filename: clickup-tasks-openapi.yml
  format: yaml
  label: ClickUp Tasks API
  slug: tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-tasks-openapi.yml
- filename: clickup-spaces-openapi.yml
  format: yaml
  label: ClickUp Spaces API
  slug: spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-spaces-openapi.yml
- filename: clickup-lists-openapi.yml
  format: yaml
  label: ClickUp Lists API
  slug: lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-lists-openapi.yml
- filename: clickup-folders-openapi.yml
  format: yaml
  label: ClickUp Folders API
  slug: folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-folders-openapi.yml
- filename: clickup-goals-openapi.yml
  format: yaml
  label: ClickUp Goals API
  slug: goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-goals-openapi.yml
- filename: clickup-comments-openapi.yml
  format: yaml
  label: ClickUp Comments API
  slug: comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-comments-openapi.yml
- filename: clickup-teams-openapi.yml
  format: yaml
  label: ClickUp Teams (Workspaces) API
  slug: teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-teams-openapi.yml
- filename: clickup-webhooks-openapi.yml
  format: yaml
  label: ClickUp Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-webhooks-openapi.yml
- filename: clickup-custom-fields-openapi.yml
  format: yaml
  label: ClickUp Custom Fields API
  slug: custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-custom-fields-openapi.yml
- filename: clickup-time-tracking-openapi.yml
  format: yaml
  label: ClickUp Time Tracking API
  slug: time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-time-tracking-openapi.yml
- filename: clickup-views-openapi.yml
  format: yaml
  label: ClickUp Views API
  slug: views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-views-openapi.yml
- filename: clickup-oauth-openapi.yml
  format: yaml
  label: ClickUp OAuth API
  slug: oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-oauth-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Clickup Authentication
name_suffix: Authentication
oauth_flows: []
overview: clickup secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: clickup
provider_slug: clickup
scheme_count: 1
schemes:
- description: ClickUp personal API token or OAuth access token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/clickup-comments-openapi.yml
  - openapi/clickup-custom-fields-openapi.yml
  - openapi/clickup-folders-openapi.yml
  - openapi/clickup-goals-openapi.yml
  - openapi/clickup-lists-openapi.yml
  - openapi/clickup-oauth-openapi.yml
  - openapi/clickup-spaces-openapi.yml
  - openapi/clickup-tasks-openapi.yml
  - openapi/clickup-teams-openapi.yml
  - openapi/clickup-time-tracking-openapi.yml
  - openapi/clickup-views-openapi.yml
  - openapi/clickup-webhooks-openapi.yml
  type: http
slug: clickup-authentication
source_filename: clickup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/clickup-comments-openapi.yml, openapi/clickup-custom-fields-openapi.yml, openapi/clickup-folders-openapi.yml,\n  openapi/clickup-goals-openapi.yml, openapi/clickup-lists-openapi.yml, openapi/clickup-oauth-openapi.yml,\n  openapi/clickup-spaces-openapi.yml, openapi/clickup-tasks-openapi.yml, openapi/clickup-teams-openapi.yml,\n  openapi/clickup-time-tracking-openapi.yml, openapi/clickup-views-openapi.yml, openapi/clickup-webhooks-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: ClickUp personal API token or OAuth access token.\n  sources:\n  - openapi/clickup-comments-openapi.yml\n  - openapi/clickup-custom-fields-openapi.yml\n  - openapi/clickup-folders-openapi.yml\n  - openapi/clickup-goals-openapi.yml\n  - openapi/clickup-lists-openapi.yml\n  - openapi/clickup-oauth-openapi.yml\n  - openapi/clickup-spaces-openapi.yml\n  - openapi/clickup-tasks-openapi.yml\n\
  \  - openapi/clickup-teams-openapi.yml\n  - openapi/clickup-time-tracking-openapi.yml\n  - openapi/clickup-views-openapi.yml\n  - openapi/clickup-webhooks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/authentication/clickup-authentication.yml
summary_line: http · 1 scheme
tags: []
---
