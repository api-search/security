---
api_key_in: []
api_specs:
- filename: gong-calls-openapi.yml
  format: yaml
  label: Gong Calls API
  slug: gong-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/gong-calls-openapi.yml
- filename: gong-users-openapi.yml
  format: yaml
  label: Gong Users API
  slug: gong-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/gong-users-openapi.yml
- filename: gong-library-openapi.yml
  format: yaml
  label: Gong Library API
  slug: gong-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/gong-library-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gong Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gong secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gong
provider_slug: gong
scheme_count: 2
schemes:
- description: 'Basic authentication using your Gong API access key and secret. Format: base64(access_key:access_secret).'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/gong-auditing-openapi.yml
  - openapi/gong-calls-openapi.yml
  - openapi/gong-crm-openapi.yml
  - openapi/gong-data-privacy-openapi.yml
  - openapi/gong-engage-openapi.yml
  - openapi/gong-engagement-openapi.yml
  - openapi/gong-library-openapi.yml
  - openapi/gong-meetings-openapi.yml
  - openapi/gong-permissions-openapi.yml
  - openapi/gong-settings-openapi.yml
  - openapi/gong-stats-openapi.yml
  - openapi/gong-users-openapi.yml
  type: http
- description: OAuth 2.0 Bearer token authentication.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gong-auditing-openapi.yml
  - openapi/gong-calls-openapi.yml
  - openapi/gong-crm-openapi.yml
  - openapi/gong-data-privacy-openapi.yml
  - openapi/gong-engage-openapi.yml
  - openapi/gong-engagement-openapi.yml
  - openapi/gong-library-openapi.yml
  - openapi/gong-meetings-openapi.yml
  - openapi/gong-permissions-openapi.yml
  - openapi/gong-settings-openapi.yml
  - openapi/gong-stats-openapi.yml
  - openapi/gong-users-openapi.yml
  type: http
slug: gong-authentication
source_filename: gong-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gong-auditing-openapi.yml, openapi/gong-calls-openapi.yml, openapi/gong-crm-openapi.yml,\n  openapi/gong-data-privacy-openapi.yml, openapi/gong-engage-openapi.yml, openapi/gong-engagement-openapi.yml,\n  openapi/gong-library-openapi.yml, openapi/gong-meetings-openapi.yml, openapi/gong-permissions-openapi.yml,\n  openapi/gong-settings-openapi.yml, openapi/gong-stats-openapi.yml, openapi/gong-users-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'Basic authentication using your Gong API access key and secret. Format: base64(access_key:access_secret).'\n  sources:\n  - openapi/gong-auditing-openapi.yml\n  - openapi/gong-calls-openapi.yml\n  - openapi/gong-crm-openapi.yml\n  - openapi/gong-data-privacy-openapi.yml\n  - openapi/gong-engage-openapi.yml\n  - openapi/gong-engagement-openapi.yml\n  - openapi/gong-library-openapi.yml\n  - openapi/gong-meetings-openapi.yml\n\
  \  - openapi/gong-permissions-openapi.yml\n  - openapi/gong-settings-openapi.yml\n  - openapi/gong-stats-openapi.yml\n  - openapi/gong-users-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer token authentication.\n  sources:\n  - openapi/gong-auditing-openapi.yml\n  - openapi/gong-calls-openapi.yml\n  - openapi/gong-crm-openapi.yml\n  - openapi/gong-data-privacy-openapi.yml\n  - openapi/gong-engage-openapi.yml\n  - openapi/gong-engagement-openapi.yml\n  - openapi/gong-library-openapi.yml\n  - openapi/gong-meetings-openapi.yml\n  - openapi/gong-permissions-openapi.yml\n  - openapi/gong-settings-openapi.yml\n  - openapi/gong-stats-openapi.yml\n  - openapi/gong-users-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/authentication/gong-authentication.yml
summary_line: http · 2 schemes
tags:
- Sales
- Revenue Intelligence
- Conversation
- Analytics
- AI
---
