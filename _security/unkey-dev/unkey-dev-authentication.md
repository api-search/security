---
api_key_in: []
api_specs:
- filename: unkey-dev-analytics-api-openapi.yml
  format: yaml
  label: Unkey analytics API
  slug: unkey-dev-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-analytics-api-openapi.yml
- filename: unkey-dev-apis-api-openapi.yml
  format: yaml
  label: Unkey apis API
  slug: unkey-dev-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-apis-api-openapi.yml
- filename: unkey-dev-deploy-api-openapi.yml
  format: yaml
  label: Unkey deploy API
  slug: unkey-dev-deploy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-deploy-api-openapi.yml
- filename: unkey-dev-identities-api-openapi.yml
  format: yaml
  label: Unkey identities API
  slug: unkey-dev-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-identities-api-openapi.yml
- filename: unkey-dev-keys-api-openapi.yml
  format: yaml
  label: Unkey keys API
  slug: unkey-dev-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-keys-api-openapi.yml
- filename: unkey-dev-liveness-api-openapi.yml
  format: yaml
  label: Unkey liveness API
  slug: unkey-dev-liveness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-liveness-api-openapi.yml
- filename: unkey-dev-permissions-api-openapi.yml
  format: yaml
  label: Unkey permissions API
  slug: unkey-dev-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-permissions-api-openapi.yml
- filename: unkey-dev-ratelimit-api-openapi.yml
  format: yaml
  label: Unkey ratelimit API
  slug: unkey-dev-ratelimit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-ratelimit-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Unkey Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unkey secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unkey
provider_slug: unkey-dev
scheme_count: 1
schemes:
- description: 'HTTP Bearer authentication with an Unkey root key, passed as `Authorization: Bearer [example key]`. Most endpoints require specific permissions on the root key.'
  name: rootKey
  scheme: bearer
  sources:
  - openapi/unkey-dev-openapi.yml
  type: http
slug: unkey-dev-authentication
source_filename: unkey-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unkey-dev-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: rootKey\n  type: http\n  scheme: bearer\n  description: 'HTTP Bearer authentication with an Unkey root key, passed as `Authorization:\n    Bearer [example key]`. Most endpoints require specific permissions on the root key.'\n  sources:\n  - openapi/unkey-dev-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/authentication/unkey-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- API Keys
- Rate Limiting
- Authentication
- Access Control
- Identity
- RBAC
- Analytics
- Open Source
---
