---
api_key_in:
- header
api_specs:
- filename: agorapulse-calendar-notes-api-openapi.yml
  format: yaml
  label: Agorapulse Calendar Notes API
  slug: agorapulse-calendar-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-calendar-notes-api-openapi.yml
- filename: agorapulse-inbox-conversations-api-openapi.yml
  format: yaml
  label: Agorapulse Inbox conversations API
  slug: agorapulse-inbox-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-inbox-conversations-api-openapi.yml
- filename: agorapulse-inbox-items-api-openapi.yml
  format: yaml
  label: Agorapulse Inbox items API
  slug: agorapulse-inbox-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-inbox-items-api-openapi.yml
- filename: agorapulse-inbox-reply-api-openapi.yml
  format: yaml
  label: Agorapulse Inbox reply API
  slug: agorapulse-inbox-reply-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-inbox-reply-api-openapi.yml
- filename: agorapulse-openapi-api-openapi.yml
  format: yaml
  label: Agorapulse OpenAPI API
  slug: agorapulse-openapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-openapi-api-openapi.yml
- filename: agorapulse-organization-api-openapi.yml
  format: yaml
  label: Agorapulse Organization API
  slug: agorapulse-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-organization-api-openapi.yml
- filename: agorapulse-profile-api-openapi.yml
  format: yaml
  label: Agorapulse Profile API
  slug: agorapulse-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-profile-api-openapi.yml
- filename: agorapulse-report-api-openapi.yml
  format: yaml
  label: Agorapulse Report API
  slug: agorapulse-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-report-api-openapi.yml
- filename: agorapulse-simple-drafts-api-openapi.yml
  format: yaml
  label: Agorapulse Simple Drafts API
  slug: agorapulse-simple-drafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-simple-drafts-api-openapi.yml
- filename: agorapulse-simple-scheduling-api-openapi.yml
  format: yaml
  label: Agorapulse Simple Scheduling API
  slug: agorapulse-simple-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-simple-scheduling-api-openapi.yml
- filename: agorapulse-studio-media-api-openapi.yml
  format: yaml
  label: Agorapulse Studio Media API
  slug: agorapulse-studio-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-studio-media-api-openapi.yml
- filename: agorapulse-workspace-api-openapi.yml
  format: yaml
  label: Agorapulse Workspace API
  slug: agorapulse-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-workspace-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Agorapulse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agorapulse secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agorapulse
provider_slug: agorapulse
scheme_count: 1
schemes:
- in: header
  name: bearerAuth
  parameter: X-API-KEY
  sources:
  - openapi/agorapulse-openapi.yml
  type: apiKey
slug: agorapulse-authentication
source_filename: agorapulse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/agorapulse-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/agorapulse-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/authentication/agorapulse-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Social Media Management
- Social Media
- CRM
- Analytics
- Publishing
- Inbox Management
- Social Listening
---
