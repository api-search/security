---
api_key_in: []
api_specs:
- filename: follow-up-boss-calls-api-openapi.yml
  format: yaml
  label: Follow Up Boss Calls API
  slug: follow-up-boss-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/follow-up-boss/refs/heads/main/openapi/follow-up-boss-calls-api-openapi.yml
- filename: follow-up-boss-deals-api-openapi.yml
  format: yaml
  label: Follow Up Boss Deals API
  slug: follow-up-boss-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/follow-up-boss/refs/heads/main/openapi/follow-up-boss-deals-api-openapi.yml
- filename: follow-up-boss-events-api-openapi.yml
  format: yaml
  label: Follow Up Boss Events API
  slug: follow-up-boss-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/follow-up-boss/refs/heads/main/openapi/follow-up-boss-events-api-openapi.yml
- filename: follow-up-boss-notes-api-openapi.yml
  format: yaml
  label: Follow Up Boss Notes API
  slug: follow-up-boss-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/follow-up-boss/refs/heads/main/openapi/follow-up-boss-notes-api-openapi.yml
- filename: follow-up-boss-people-api-openapi.yml
  format: yaml
  label: Follow Up Boss People API
  slug: follow-up-boss-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/follow-up-boss/refs/heads/main/openapi/follow-up-boss-people-api-openapi.yml
- filename: follow-up-boss-tasks-api-openapi.yml
  format: yaml
  label: Follow Up Boss Tasks API
  slug: follow-up-boss-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/follow-up-boss/refs/heads/main/openapi/follow-up-boss-tasks-api-openapi.yml
- filename: follow-up-boss-textmessages-api-openapi.yml
  format: yaml
  label: Follow Up Boss TextMessages API
  slug: follow-up-boss-textmessages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/follow-up-boss/refs/heads/main/openapi/follow-up-boss-textmessages-api-openapi.yml
- filename: follow-up-boss-webhooks-api-openapi.yml
  format: yaml
  label: Follow Up Boss Webhooks API
  slug: follow-up-boss-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/follow-up-boss/refs/heads/main/openapi/follow-up-boss-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Follow Up Boss Authentication
name_suffix: Authentication
oauth_flows: []
overview: Follow Up Boss secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Follow Up Boss
provider_slug: follow-up-boss
scheme_count: 1
schemes:
- description: HTTP Basic auth with the Follow Up Boss API key as the username and a blank password
  name: basicAuth
  scheme: basic
  sources:
  - openapi/follow-up-boss-openapi.yml
  type: http
slug: follow-up-boss-authentication
source_filename: follow-up-boss-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/follow-up-boss-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth with the Follow Up Boss API key as the username and a blank password\n  sources:\n  - openapi/follow-up-boss-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/follow-up-boss/refs/heads/main/authentication/follow-up-boss-authentication.yml
summary_line: http · 1 scheme
tags:
- Real Estate
- CRM
- Lead Management
- Sales Automation
- Follow Up
- Pipeline Management
---
