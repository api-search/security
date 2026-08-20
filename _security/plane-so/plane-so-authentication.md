---
api_key_in:
- header
api_specs:
- filename: plane-so-cycle-work-items-api-openapi.yml
  format: yaml
  label: Plane Cycle Work Items API
  slug: plane-so-cycle-work-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-cycle-work-items-api-openapi.yml
- filename: plane-so-cycles-api-openapi.yml
  format: yaml
  label: Plane Cycles API
  slug: plane-so-cycles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-cycles-api-openapi.yml
- filename: plane-so-labels-api-openapi.yml
  format: yaml
  label: Plane Labels API
  slug: plane-so-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-labels-api-openapi.yml
- filename: plane-so-members-api-openapi.yml
  format: yaml
  label: Plane Members API
  slug: plane-so-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-members-api-openapi.yml
- filename: plane-so-module-work-items-api-openapi.yml
  format: yaml
  label: Plane Module Work Items API
  slug: plane-so-module-work-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-module-work-items-api-openapi.yml
- filename: plane-so-modules-api-openapi.yml
  format: yaml
  label: Plane Modules API
  slug: plane-so-modules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-modules-api-openapi.yml
- filename: plane-so-projects-api-openapi.yml
  format: yaml
  label: Plane Projects API
  slug: plane-so-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-projects-api-openapi.yml
- filename: plane-so-states-api-openapi.yml
  format: yaml
  label: Plane States API
  slug: plane-so-states-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-states-api-openapi.yml
- filename: plane-so-work-item-comments-api-openapi.yml
  format: yaml
  label: Plane Work Item Comments API
  slug: plane-so-work-item-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-work-item-comments-api-openapi.yml
- filename: plane-so-work-item-links-api-openapi.yml
  format: yaml
  label: Plane Work Item Links API
  slug: plane-so-work-item-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-work-item-links-api-openapi.yml
- filename: plane-so-work-items-api-openapi.yml
  format: yaml
  label: Plane Work Items API
  slug: plane-so-work-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-work-items-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Plane So Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plane secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Plane
provider_slug: plane-so
scheme_count: 1
schemes:
- description: API key generated from your Plane workspace settings. Pass it in the X-API-Key header on every request.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/plane-so-openapi.yml
  type: apiKey
slug: plane-so-authentication
source_filename: plane-so-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/plane-so-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key generated from your Plane workspace settings. Pass it in the X-API-Key\n    header on every request.\n  sources:\n  - openapi/plane-so-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/authentication/plane-so-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Project Management
- Issue Tracking
- Work Management
- Open-Source
- Productivity
---
