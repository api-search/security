---
api_key_in:
- query
api_specs:
- filename: ghost-org-openapi.yml
  format: yaml
  label: Ghost Content API
  slug: ghost-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-openapi.yml
- filename: ghost-org-openapi.yml
  format: yaml
  label: Ghost Admin Posts API
  slug: ghost-admin-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-openapi.yml
- filename: ghost-org-openapi.yml
  format: yaml
  label: Ghost Admin Pages API
  slug: ghost-admin-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-openapi.yml
- filename: ghost-org-openapi.yml
  format: yaml
  label: Ghost Admin Members API
  slug: ghost-admin-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-openapi.yml
- filename: ghost-org-openapi.yml
  format: yaml
  label: Ghost Admin Tags and Labels API
  slug: ghost-admin-tags-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-openapi.yml
- filename: ghost-org-openapi.yml
  format: yaml
  label: Ghost Admin Tiers and Offers API
  slug: ghost-admin-tiers-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-openapi.yml
- filename: ghost-org-openapi.yml
  format: yaml
  label: Ghost Admin Newsletters API
  slug: ghost-admin-newsletters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-openapi.yml
- filename: ghost-org-openapi.yml
  format: yaml
  label: Ghost Admin Users and Site API
  slug: ghost-admin-users-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-openapi.yml
- filename: ghost-org-openapi.yml
  format: yaml
  label: Ghost Admin Media and Themes API
  slug: ghost-admin-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-openapi.yml
- filename: ghost-org-openapi.yml
  format: yaml
  label: Ghost Admin Webhooks API
  slug: ghost-admin-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ghost Org Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ghost secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ghost
provider_slug: ghost-org
scheme_count: 2
schemes:
- description: Content API key from a Custom Integration, passed as the `key` query parameter. Safe for browser use; grants read-only access to public data.
  in: query
  name: contentApiKey
  parameter: key
  sources:
  - openapi/ghost-org-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: 'Admin API access. An Admin API key (id:secret) is used to sign a short-lived JWT sent as `Authorization: Ghost {token}`. A staff access token or an authenticated user session may also be used.'
  name: adminJwt
  scheme: bearer
  sources:
  - openapi/ghost-org-openapi.yml
  type: http
slug: ghost-org-authentication
source_filename: ghost-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ghost-org-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: contentApiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: Content API key from a Custom Integration, passed as the `key` query parameter.\n    Safe for browser use; grants read-only access to public data.\n  sources:\n  - openapi/ghost-org-openapi.yml\n- name: adminJwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Admin API access. An Admin API key (id:secret) is used to sign a short-lived\n    JWT sent as `Authorization: Ghost {token}`. A staff access token or an authenticated user\n    session may also be used.'\n  sources:\n  - openapi/ghost-org-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/authentication/ghost-org-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Publishing
- Newsletters
- Memberships
- Subscriptions
- CMS
- Open Source
- Content
---
