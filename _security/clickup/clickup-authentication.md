---
api_key_in: []
api_specs:
- filename: clickup-authorization-api-openapi.yml
  format: yaml
  label: clickup Authorization API
  slug: clickup-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-authorization-api-openapi.yml
- filename: clickup-comments-api-openapi.yml
  format: yaml
  label: clickup Comments API
  slug: clickup-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-comments-api-openapi.yml
- filename: clickup-custom-fields-api-openapi.yml
  format: yaml
  label: clickup Custom Fields API
  slug: clickup-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-custom-fields-api-openapi.yml
- filename: clickup-folders-api-openapi.yml
  format: yaml
  label: clickup Folders API
  slug: clickup-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-folders-api-openapi.yml
- filename: clickup-goals-api-openapi.yml
  format: yaml
  label: clickup Goals API
  slug: clickup-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-goals-api-openapi.yml
- filename: clickup-lists-api-openapi.yml
  format: yaml
  label: clickup Lists API
  slug: clickup-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-lists-api-openapi.yml
- filename: clickup-oauth-api-openapi.yml
  format: yaml
  label: clickup OAuth API
  slug: clickup-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-oauth-api-openapi.yml
- filename: clickup-spaces-api-openapi.yml
  format: yaml
  label: clickup Spaces API
  slug: clickup-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-spaces-api-openapi.yml
- filename: clickup-tasks-api-openapi.yml
  format: yaml
  label: clickup Tasks API
  slug: clickup-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-tasks-api-openapi.yml
- filename: clickup-teams-api-openapi.yml
  format: yaml
  label: clickup Teams API
  slug: clickup-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-teams-api-openapi.yml
- filename: clickup-time-tracking-api-openapi.yml
  format: yaml
  label: clickup Time Tracking API
  slug: clickup-time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-time-tracking-api-openapi.yml
- filename: clickup-views-api-openapi.yml
  format: yaml
  label: clickup Views API
  slug: clickup-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-views-api-openapi.yml
- filename: clickup-webhooks-api-openapi.yml
  format: yaml
  label: clickup Webhooks API
  slug: clickup-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-webhooks-api-openapi.yml
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
