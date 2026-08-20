---
api_key_in:
- query
api_specs:
- filename: ghost-org-admin-images-api-openapi.yml
  format: yaml
  label: Ghost Admin - Images API
  slug: ghost-org-admin-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-admin-images-api-openapi.yml
- filename: ghost-org-admin-labels-api-openapi.yml
  format: yaml
  label: Ghost Admin - Labels API
  slug: ghost-org-admin-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-admin-labels-api-openapi.yml
- filename: ghost-org-admin-members-api-openapi.yml
  format: yaml
  label: Ghost Admin - Members API
  slug: ghost-org-admin-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-admin-members-api-openapi.yml
- filename: ghost-org-admin-newsletters-api-openapi.yml
  format: yaml
  label: Ghost Admin - Newsletters API
  slug: ghost-org-admin-newsletters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-admin-newsletters-api-openapi.yml
- filename: ghost-org-admin-offers-api-openapi.yml
  format: yaml
  label: Ghost Admin - Offers API
  slug: ghost-org-admin-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-admin-offers-api-openapi.yml
- filename: ghost-org-admin-pages-api-openapi.yml
  format: yaml
  label: Ghost Admin - Pages API
  slug: ghost-org-admin-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-admin-pages-api-openapi.yml
- filename: ghost-org-admin-posts-api-openapi.yml
  format: yaml
  label: Ghost Admin - Posts API
  slug: ghost-org-admin-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-admin-posts-api-openapi.yml
- filename: ghost-org-admin-site-api-openapi.yml
  format: yaml
  label: Ghost Admin - Site API
  slug: ghost-org-admin-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-admin-site-api-openapi.yml
- filename: ghost-org-admin-tags-api-openapi.yml
  format: yaml
  label: Ghost Admin - Tags API
  slug: ghost-org-admin-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-admin-tags-api-openapi.yml
- filename: ghost-org-admin-themes-api-openapi.yml
  format: yaml
  label: Ghost Admin - Themes API
  slug: ghost-org-admin-themes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-admin-themes-api-openapi.yml
- filename: ghost-org-admin-tiers-api-openapi.yml
  format: yaml
  label: Ghost Admin - Tiers API
  slug: ghost-org-admin-tiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-admin-tiers-api-openapi.yml
- filename: ghost-org-admin-users-api-openapi.yml
  format: yaml
  label: Ghost Admin - Users API
  slug: ghost-org-admin-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-admin-users-api-openapi.yml
- filename: ghost-org-admin-webhooks-api-openapi.yml
  format: yaml
  label: Ghost Admin - Webhooks API
  slug: ghost-org-admin-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-admin-webhooks-api-openapi.yml
- filename: ghost-org-content-authors-api-openapi.yml
  format: yaml
  label: Ghost Content - Authors API
  slug: ghost-org-content-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-content-authors-api-openapi.yml
- filename: ghost-org-content-pages-api-openapi.yml
  format: yaml
  label: Ghost Content - Pages API
  slug: ghost-org-content-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-content-pages-api-openapi.yml
- filename: ghost-org-content-posts-api-openapi.yml
  format: yaml
  label: Ghost Content - Posts API
  slug: ghost-org-content-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-content-posts-api-openapi.yml
- filename: ghost-org-content-settings-api-openapi.yml
  format: yaml
  label: Ghost Content - Settings API
  slug: ghost-org-content-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-content-settings-api-openapi.yml
- filename: ghost-org-content-tags-api-openapi.yml
  format: yaml
  label: Ghost Content - Tags API
  slug: ghost-org-content-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-content-tags-api-openapi.yml
- filename: ghost-org-content-tiers-api-openapi.yml
  format: yaml
  label: Ghost Content - Tiers API
  slug: ghost-org-content-tiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/openapi/ghost-org-content-tiers-api-openapi.yml
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
  - openapi/ghost-org-admin-images-api-openapi.yml
  - openapi/ghost-org-admin-labels-api-openapi.yml
  - openapi/ghost-org-admin-members-api-openapi.yml
  - openapi/ghost-org-admin-newsletters-api-openapi.yml
  - openapi/ghost-org-admin-offers-api-openapi.yml
  - openapi/ghost-org-admin-pages-api-openapi.yml
  - openapi/ghost-org-admin-posts-api-openapi.yml
  - openapi/ghost-org-admin-site-api-openapi.yml
  - openapi/ghost-org-admin-tags-api-openapi.yml
  - openapi/ghost-org-admin-themes-api-openapi.yml
  - openapi/ghost-org-admin-tiers-api-openapi.yml
  - openapi/ghost-org-admin-users-api-openapi.yml
  - openapi/ghost-org-admin-webhooks-api-openapi.yml
  - openapi/ghost-org-content-authors-api-openapi.yml
  - openapi/ghost-org-content-pages-api-openapi.yml
  - openapi/ghost-org-content-posts-api-openapi.yml
  - openapi/ghost-org-content-settings-api-openapi.yml
  - openapi/ghost-org-content-tags-api-openapi.yml
  - openapi/ghost-org-content-tiers-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: 'Admin API access. An Admin API key (id:secret) is used to sign a short-lived JWT sent as `Authorization: Ghost {token}`. A staff access token or an authenticated user session may also be used.'
  name: adminJwt
  scheme: bearer
  sources:
  - openapi/ghost-org-admin-images-api-openapi.yml
  - openapi/ghost-org-admin-labels-api-openapi.yml
  - openapi/ghost-org-admin-members-api-openapi.yml
  - openapi/ghost-org-admin-newsletters-api-openapi.yml
  - openapi/ghost-org-admin-offers-api-openapi.yml
  - openapi/ghost-org-admin-pages-api-openapi.yml
  - openapi/ghost-org-admin-posts-api-openapi.yml
  - openapi/ghost-org-admin-site-api-openapi.yml
  - openapi/ghost-org-admin-tags-api-openapi.yml
  - openapi/ghost-org-admin-themes-api-openapi.yml
  - openapi/ghost-org-admin-tiers-api-openapi.yml
  - openapi/ghost-org-admin-users-api-openapi.yml
  - openapi/ghost-org-admin-webhooks-api-openapi.yml
  - openapi/ghost-org-authors-api-openapi.yml
  - openapi/ghost-org-content-authors-api-openapi.yml
  - openapi/ghost-org-content-pages-api-openapi.yml
  - openapi/ghost-org-content-posts-api-openapi.yml
  - openapi/ghost-org-content-settings-api-openapi.yml
  - openapi/ghost-org-content-tags-api-openapi.yml
  - openapi/ghost-org-content-tiers-api-openapi.yml
  - openapi/ghost-org-images-api-openapi.yml
  - openapi/ghost-org-members-api-openapi.yml
  - openapi/ghost-org-newsletters-api-openapi.yml
  - openapi/ghost-org-offers-api-openapi.yml
  - openapi/ghost-org-pages-api-openapi.yml
  - openapi/ghost-org-posts-api-openapi.yml
  - openapi/ghost-org-settings-api-openapi.yml
  - openapi/ghost-org-site-api-openapi.yml
  - openapi/ghost-org-tags-api-openapi.yml
  - openapi/ghost-org-themes-api-openapi.yml
  - openapi/ghost-org-tiers-api-openapi.yml
  - openapi/ghost-org-users-api-openapi.yml
  - openapi/ghost-org-webhooks-api-openapi.yml
  type: http
slug: ghost-org-authentication
source_filename: ghost-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/ghost-org-admin-images-api-openapi.yml, openapi/ghost-org-admin-labels-api-openapi.yml,\n  openapi/ghost-org-admin-members-api-openapi.yml, openapi/ghost-org-admin-newsletters-api-openapi.yml,\n  openapi/ghost-org-admin-offers-api-openapi.yml, openapi/ghost-org-admin-pages-api-openapi.yml,\n  openapi/ghost-org-admin-posts-api-openapi.yml, openapi/ghost-org-admin-site-api-openapi.yml,\n  openapi/ghost-org-admin-tags-api-openapi.yml, openapi/ghost-org-admin-themes-api-openapi.yml,\n  openapi/ghost-org-admin-tiers-api-openapi.yml, openapi/ghost-org-admin-users-api-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: contentApiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: Content API key from a Custom Integration, passed as the `key` query parameter.\n    Safe for browser use; grants read-only access to public data.\n  sources:\n  - openapi/ghost-org-admin-images-api-openapi.yml\n\
  \  - openapi/ghost-org-admin-labels-api-openapi.yml\n  - openapi/ghost-org-admin-members-api-openapi.yml\n  - openapi/ghost-org-admin-newsletters-api-openapi.yml\n  - openapi/ghost-org-admin-offers-api-openapi.yml\n  - openapi/ghost-org-admin-pages-api-openapi.yml\n  - openapi/ghost-org-admin-posts-api-openapi.yml\n  - openapi/ghost-org-admin-site-api-openapi.yml\n  - openapi/ghost-org-admin-tags-api-openapi.yml\n  - openapi/ghost-org-admin-themes-api-openapi.yml\n  - openapi/ghost-org-admin-tiers-api-openapi.yml\n  - openapi/ghost-org-admin-users-api-openapi.yml\n  - openapi/ghost-org-admin-webhooks-api-openapi.yml\n  - openapi/ghost-org-content-authors-api-openapi.yml\n  - openapi/ghost-org-content-pages-api-openapi.yml\n  - openapi/ghost-org-content-posts-api-openapi.yml\n  - openapi/ghost-org-content-settings-api-openapi.yml\n  - openapi/ghost-org-content-tags-api-openapi.yml\n  - openapi/ghost-org-content-tiers-api-openapi.yml\n- name: adminJwt\n  type: http\n  scheme: bearer\n  bearerFormat:\
  \ JWT\n  description: 'Admin API access. An Admin API key (id:secret) is used to sign a short-lived\n    JWT sent as `Authorization: Ghost {token}`. A staff access token or an authenticated user\n    session may also be used.'\n  sources:\n  - openapi/ghost-org-admin-images-api-openapi.yml\n  - openapi/ghost-org-admin-labels-api-openapi.yml\n  - openapi/ghost-org-admin-members-api-openapi.yml\n  - openapi/ghost-org-admin-newsletters-api-openapi.yml\n  - openapi/ghost-org-admin-offers-api-openapi.yml\n  - openapi/ghost-org-admin-pages-api-openapi.yml\n  - openapi/ghost-org-admin-posts-api-openapi.yml\n  - openapi/ghost-org-admin-site-api-openapi.yml\n  - openapi/ghost-org-admin-tags-api-openapi.yml\n  - openapi/ghost-org-admin-themes-api-openapi.yml\n  - openapi/ghost-org-admin-tiers-api-openapi.yml\n  - openapi/ghost-org-admin-users-api-openapi.yml\n  - openapi/ghost-org-admin-webhooks-api-openapi.yml\n  - openapi/ghost-org-authors-api-openapi.yml\n  - openapi/ghost-org-content-authors-api-openapi.yml\n\
  \  - openapi/ghost-org-content-pages-api-openapi.yml\n  - openapi/ghost-org-content-posts-api-openapi.yml\n  - openapi/ghost-org-content-settings-api-openapi.yml\n  - openapi/ghost-org-content-tags-api-openapi.yml\n  - openapi/ghost-org-content-tiers-api-openapi.yml\n  - openapi/ghost-org-images-api-openapi.yml\n  - openapi/ghost-org-members-api-openapi.yml\n  - openapi/ghost-org-newsletters-api-openapi.yml\n  - openapi/ghost-org-offers-api-openapi.yml\n  - openapi/ghost-org-pages-api-openapi.yml\n  - openapi/ghost-org-posts-api-openapi.yml\n  - openapi/ghost-org-settings-api-openapi.yml\n  - openapi/ghost-org-site-api-openapi.yml\n  - openapi/ghost-org-tags-api-openapi.yml\n  - openapi/ghost-org-themes-api-openapi.yml\n  - openapi/ghost-org-tiers-api-openapi.yml\n  - openapi/ghost-org-users-api-openapi.yml\n  - openapi/ghost-org-webhooks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ghost-org/refs/heads/main/authentication/ghost-org-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Publishing
- Newsletters
- Memberships
- Subscription
- CMS
- Open-Source
- Content
---
