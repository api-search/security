---
api_key_in:
- header
api_specs:
- filename: release-openapi-original.json
  format: json
  label: Release Platform API
  slug: release-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/release/refs/heads/main/openapi/release-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Release Authentication
name_suffix: Authentication
oauth_flows: []
overview: Release secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Release
provider_slug: release
scheme_count: 2
schemes:
- description: User's email address for authentication
  in: header
  name: userEmail
  parameter: X-User-Email
  sources:
  - openapi/release-openapi-original.json
  type: apiKey
- description: User's authentication token (from ~/.release.yaml)
  in: header
  name: userToken
  parameter: X-User-Token
  sources:
  - openapi/release-openapi-original.json
  type: apiKey
slug: release-authentication
source_filename: release-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/release-openapi-original.json\ndocs: https://docs.release.com/reference-documentation/release-api/authentication.md\nnotes: >-\n  Two apiKey header credentials are required together (X-User-Email + X-User-Token),\n  sourced from ~/.release.yaml (populated by `release auth login`). Some Platform API\n  endpoints instead use account-level headers X-Account-ID + X-Account-Token (found in\n  Account Settings > Account Info); AI Sandbox and GraphQL APIs always use user auth.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  account_level_headers:\n  - X-Account-ID\n  - X-Account-Token\nschemes:\n- name: userEmail\n  type: apiKey\n  in: header\n  parameter: X-User-Email\n  description: User's email address for authentication\n  sources:\n  - openapi/release-openapi-original.json\n- name: userToken\n  type: apiKey\n  in: header\n  parameter: X-User-Token\n  description: User's authentication token (from ~/.release.yaml)\n\
  \  sources:\n  - openapi/release-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/release/refs/heads/main/authentication/release-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Developer Tools
- Ephemeral Environments
- Platform Engineering
- Deployment
- Kubernetes
- Environments as a Service
- DevOps
- CI/CD
- AI Sandbox
---
