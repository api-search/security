---
api_key_in: []
api_specs:
- filename: lemmy-account-api-openapi.yml
  format: yaml
  label: Lemmy Account API
  slug: lemmy-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemmy/refs/heads/main/openapi/lemmy-account-api-openapi.yml
- filename: lemmy-admin-api-openapi.yml
  format: yaml
  label: Lemmy Admin API
  slug: lemmy-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemmy/refs/heads/main/openapi/lemmy-admin-api-openapi.yml
- filename: lemmy-authentication-api-openapi.yml
  format: yaml
  label: Lemmy Authentication API
  slug: lemmy-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemmy/refs/heads/main/openapi/lemmy-authentication-api-openapi.yml
- filename: lemmy-comment-api-openapi.yml
  format: yaml
  label: Lemmy Comment API
  slug: lemmy-comment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemmy/refs/heads/main/openapi/lemmy-comment-api-openapi.yml
- filename: lemmy-community-api-openapi.yml
  format: yaml
  label: Lemmy Community API
  slug: lemmy-community-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemmy/refs/heads/main/openapi/lemmy-community-api-openapi.yml
- filename: lemmy-federation-api-openapi.yml
  format: yaml
  label: Lemmy Federation API
  slug: lemmy-federation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemmy/refs/heads/main/openapi/lemmy-federation-api-openapi.yml
- filename: lemmy-images-api-openapi.yml
  format: yaml
  label: Lemmy Images API
  slug: lemmy-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemmy/refs/heads/main/openapi/lemmy-images-api-openapi.yml
- filename: lemmy-notifications-api-openapi.yml
  format: yaml
  label: Lemmy Notifications API
  slug: lemmy-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemmy/refs/heads/main/openapi/lemmy-notifications-api-openapi.yml
- filename: lemmy-person-api-openapi.yml
  format: yaml
  label: Lemmy Person API
  slug: lemmy-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemmy/refs/heads/main/openapi/lemmy-person-api-openapi.yml
- filename: lemmy-post-api-openapi.yml
  format: yaml
  label: Lemmy Post API
  slug: lemmy-post-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemmy/refs/heads/main/openapi/lemmy-post-api-openapi.yml
- filename: lemmy-private-messages-api-openapi.yml
  format: yaml
  label: Lemmy Private Messages API
  slug: lemmy-private-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemmy/refs/heads/main/openapi/lemmy-private-messages-api-openapi.yml
- filename: lemmy-reports-api-openapi.yml
  format: yaml
  label: Lemmy Reports API
  slug: lemmy-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemmy/refs/heads/main/openapi/lemmy-reports-api-openapi.yml
- filename: lemmy-search-api-openapi.yml
  format: yaml
  label: Lemmy Search API
  slug: lemmy-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemmy/refs/heads/main/openapi/lemmy-search-api-openapi.yml
- filename: lemmy-site-api-openapi.yml
  format: yaml
  label: Lemmy Site API
  slug: lemmy-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemmy/refs/heads/main/openapi/lemmy-site-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lemmy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lemmy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lemmy
provider_slug: lemmy
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
slug: lemmy-authentication
source_filename: lemmy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemmy/refs/heads/main/authentication/lemmy-authentication.yml
summary_line: http · 1 scheme
tags:
- Communities
- Federated
- Fediverse
- Link Aggregator
- Open-Source
- Social Networks
---
