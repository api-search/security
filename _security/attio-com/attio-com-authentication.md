---
api_key_in: []
api_specs:
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio Objects API
  slug: attio-com-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio Records API
  slug: attio-com-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio Attributes API
  slug: attio-com-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio Lists API
  slug: attio-com-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio List Entries API
  slug: attio-com-list-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio Deals API
  slug: attio-com-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio Notes API
  slug: attio-com-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio Tasks API
  slug: attio-com-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio Comments and Threads API
  slug: attio-com-comments-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio Webhooks API
  slug: attio-com-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio Workspace Members API
  slug: attio-com-workspace-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
- filename: attio-com-openapi.yml
  format: yaml
  label: Attio Meta / Self API
  slug: attio-com-meta-self-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/openapi/attio-com-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Attio Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Attio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Attio
provider_slug: attio-com
scheme_count: 1
schemes:
- description: Attio access token (API key or OAuth 2.0 bearer token) with the required scopes.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/attio-com-openapi.yml
  type: http
slug: attio-com-authentication
source_filename: attio-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/attio-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Attio access token (API key or OAuth 2.0 bearer token) with the required scopes.\n  sources:\n  - openapi/attio-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attio-com/refs/heads/main/authentication/attio-com-authentication.yml
summary_line: http · 1 scheme
tags:
- CRM
- Customer Relationship Management
- AI
- Sales
- Data Model
- Objects and Records
---
