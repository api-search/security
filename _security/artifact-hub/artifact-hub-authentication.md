---
api_key_in:
- cookie
- header
api_specs:
- filename: artifact-hub-openapi.yml
  format: yaml
  label: Artifact Hub API
  slug: artifact-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifact-hub/refs/heads/main/openapi/artifact-hub-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Artifact Hub Authentication
name_suffix: Authentication
oauth_flows: []
overview: Artifact Hub secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Artifact Hub
provider_slug: artifact-hub
scheme_count: 2
schemes:
- description: 'API key authentication. Clients send the API key ID in the

    `X-API-KEY-ID` header and the API key secret in the

    `X-API-KEY-SECRET` header.'
  in: header
  name: apiKey
  parameter: X-API-KEY-ID
  sources:
  - openapi/artifact-hub-openapi.yml
  type: apiKey
- description: Session cookie obtained from /api/v1/users/login
  in: cookie
  name: cookieAuth
  parameter: session
  sources:
  - openapi/artifact-hub-openapi.yml
  type: apiKey
slug: artifact-hub-authentication
source_filename: artifact-hub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/artifact-hub-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY-ID\n  description: |-\n    API key authentication. Clients send the API key ID in the\n    `X-API-KEY-ID` header and the API key secret in the\n    `X-API-KEY-SECRET` header.\n  sources:\n  - openapi/artifact-hub-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: session\n  description: Session cookie obtained from /api/v1/users/login\n  sources:\n  - openapi/artifact-hub-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artifact-hub/refs/heads/main/authentication/artifact-hub-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Cloud Native
- CNCF
- Helm Charts
- Package Registry
- Discovery
- Open Source
---
