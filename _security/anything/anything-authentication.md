---
api_key_in: []
api_specs:
- filename: anything-assets-api-openapi.yml
  format: yaml
  label: Anything Assets API
  slug: anything-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-assets-api-openapi.yml
- filename: anything-databases-api-openapi.yml
  format: yaml
  label: Anything Databases API
  slug: anything-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-databases-api-openapi.yml
- filename: anything-deployments-api-openapi.yml
  format: yaml
  label: Anything Deployments API
  slug: anything-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-deployments-api-openapi.yml
- filename: anything-domains-api-openapi.yml
  format: yaml
  label: Anything Domains API
  slug: anything-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-domains-api-openapi.yml
- filename: anything-files-api-openapi.yml
  format: yaml
  label: Anything Files API
  slug: anything-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-files-api-openapi.yml
- filename: anything-generation-api-openapi.yml
  format: yaml
  label: Anything Generation API
  slug: anything-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-generation-api-openapi.yml
- filename: anything-logs-api-openapi.yml
  format: yaml
  label: Anything Logs API
  slug: anything-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-logs-api-openapi.yml
- filename: anything-messages-api-openapi.yml
  format: yaml
  label: Anything Messages API
  slug: anything-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-messages-api-openapi.yml
- filename: anything-mobile-api-openapi.yml
  format: yaml
  label: Anything Mobile API
  slug: anything-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-mobile-api-openapi.yml
- filename: anything-organizations-api-openapi.yml
  format: yaml
  label: Anything Organizations API
  slug: anything-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-organizations-api-openapi.yml
- filename: anything-projects-api-openapi.yml
  format: yaml
  label: Anything Projects API
  slug: anything-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-projects-api-openapi.yml
- filename: anything-secrets-api-openapi.yml
  format: yaml
  label: Anything Secrets API
  slug: anything-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-secrets-api-openapi.yml
- filename: anything-settings-api-openapi.yml
  format: yaml
  label: Anything Settings API
  slug: anything-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-settings-api-openapi.yml
- filename: anything-user-api-openapi.yml
  format: yaml
  label: Anything User API
  slug: anything-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-user-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Anything Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anything secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Anything
provider_slug: anything
scheme_count: 1
schemes:
- description: 'Use your Anything API key as the Basic auth username and leave the password empty. Example credentials: anything_xxx:'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/anything-openapi-original.json
  type: http
slug: anything-authentication
source_filename: anything-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/anything-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'Use your Anything API key as the Basic auth username and leave the password\n    empty. Example credentials: anything_xxx:'\n  sources:\n  - openapi/anything-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/authentication/anything-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai Ml
- App Builder
- Low Code
- No Code
- Developer Tools
- AI Agents
- Mobile
---
