---
api_key_in:
- query
api_specs:
- filename: ghost-authors-api-openapi.yml
  format: yaml
  label: Ghost Authors API
  slug: ghost-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-authors-api-openapi.yml
- filename: ghost-images-api-openapi.yml
  format: yaml
  label: Ghost Images API
  slug: ghost-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-images-api-openapi.yml
- filename: ghost-members-api-openapi.yml
  format: yaml
  label: Ghost Members API
  slug: ghost-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-members-api-openapi.yml
- filename: ghost-newsletters-api-openapi.yml
  format: yaml
  label: Ghost Newsletters API
  slug: ghost-newsletters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-newsletters-api-openapi.yml
- filename: ghost-offers-api-openapi.yml
  format: yaml
  label: Ghost Offers API
  slug: ghost-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-offers-api-openapi.yml
- filename: ghost-pages-api-openapi.yml
  format: yaml
  label: Ghost Pages API
  slug: ghost-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-pages-api-openapi.yml
- filename: ghost-posts-api-openapi.yml
  format: yaml
  label: Ghost Posts API
  slug: ghost-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-posts-api-openapi.yml
- filename: ghost-settings-api-openapi.yml
  format: yaml
  label: Ghost Settings API
  slug: ghost-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-settings-api-openapi.yml
- filename: ghost-site-api-openapi.yml
  format: yaml
  label: Ghost Site API
  slug: ghost-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-site-api-openapi.yml
- filename: ghost-tags-api-openapi.yml
  format: yaml
  label: Ghost Tags API
  slug: ghost-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-tags-api-openapi.yml
- filename: ghost-themes-api-openapi.yml
  format: yaml
  label: Ghost Themes API
  slug: ghost-themes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-themes-api-openapi.yml
- filename: ghost-tiers-api-openapi.yml
  format: yaml
  label: Ghost Tiers API
  slug: ghost-tiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-tiers-api-openapi.yml
- filename: ghost-users-api-openapi.yml
  format: yaml
  label: Ghost Users API
  slug: ghost-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-users-api-openapi.yml
- filename: ghost-webhooks-api-openapi.yml
  format: yaml
  label: Ghost Webhooks API
  slug: ghost-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ghost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ghost secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ghost
provider_slug: ghost
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: JSON Web Token generated from an Admin API key. The key is split into an ID and secret at the colon separator. The ID is used as the kid header and the secret is used to sign the token with HS256.
  name: adminApiToken
  scheme: bearer
  sources:
  - openapi/ghost-admin-api-openapi.yml
  type: http
- description: Content API key obtained from a custom integration in Ghost Admin. Content API keys are safe for use in browsers and other insecure environments as they only provide access to public data.
  in: query
  name: contentApiKey
  parameter: key
  sources:
  - openapi/ghost-content-api-openapi.yml
  type: apiKey
slug: ghost-authentication
source_filename: ghost-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ghost-admin-api-openapi.yml, openapi/ghost-content-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: adminApiToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JSON Web Token generated from an Admin API key. The key is split into an ID and\n    secret at the colon separator. The ID is used as the kid header and the secret is used to\n    sign the token with HS256.\n  sources:\n  - openapi/ghost-admin-api-openapi.yml\n- name: contentApiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: Content API key obtained from a custom integration in Ghost Admin. Content API\n    keys are safe for use in browsers and other insecure environments as they only provide access\n    to public data.\n  sources:\n  - openapi/ghost-content-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/authentication/ghost-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Publishing
- Newsletters
- Memberships
- Content
- Open Source
---
