---
api_key_in:
- header
api_specs:
- filename: plane-so-openapi.yml
  format: yaml
  label: Plane Projects API
  slug: projects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-openapi.yml
- filename: plane-so-openapi.yml
  format: yaml
  label: Plane Issues API
  slug: issues
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-openapi.yml
- filename: plane-so-openapi.yml
  format: yaml
  label: Plane Cycles API
  slug: cycles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-openapi.yml
- filename: plane-so-openapi.yml
  format: yaml
  label: Plane Modules API
  slug: modules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-openapi.yml
- filename: plane-so-openapi.yml
  format: yaml
  label: Plane States & Labels API
  slug: states-labels
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-openapi.yml
- filename: plane-so-openapi.yml
  format: yaml
  label: Plane Members API
  slug: members
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-openapi.yml
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
- Open Source
- Productivity
---
