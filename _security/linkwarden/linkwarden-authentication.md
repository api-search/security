---
anonymous_access: false
api_key_in: []
api_specs:
- filename: linkwarden-archives-api-openapi.yml
  format: yaml
  label: Linkwarden Archives API
  slug: linkwarden-archives-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkwarden/openapi/linkwarden-archives-api-openapi.yml
- filename: linkwarden-auth-api-openapi.yml
  format: yaml
  label: Linkwarden Auth API
  slug: linkwarden-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkwarden/openapi/linkwarden-auth-api-openapi.yml
- filename: linkwarden-avatar-api-openapi.yml
  format: yaml
  label: Linkwarden Avatar API
  slug: linkwarden-avatar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkwarden/openapi/linkwarden-avatar-api-openapi.yml
- filename: linkwarden-collections-api-openapi.yml
  format: yaml
  label: Linkwarden Collections API
  slug: linkwarden-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkwarden/openapi/linkwarden-collections-api-openapi.yml
- filename: linkwarden-config-api-openapi.yml
  format: yaml
  label: Linkwarden Config API
  slug: linkwarden-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkwarden/openapi/linkwarden-config-api-openapi.yml
- filename: linkwarden-dashboard-api-openapi.yml
  format: yaml
  label: Linkwarden Dashboard API
  slug: linkwarden-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkwarden/openapi/linkwarden-dashboard-api-openapi.yml
- filename: linkwarden-favicon-api-openapi.yml
  format: yaml
  label: Linkwarden Favicon API
  slug: linkwarden-favicon-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkwarden/openapi/linkwarden-favicon-api-openapi.yml
- filename: linkwarden-highlights-api-openapi.yml
  format: yaml
  label: Linkwarden Highlights API
  slug: linkwarden-highlights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkwarden/openapi/linkwarden-highlights-api-openapi.yml
- filename: linkwarden-links-api-openapi.yml
  format: yaml
  label: Linkwarden Links API
  slug: linkwarden-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkwarden/openapi/linkwarden-links-api-openapi.yml
- filename: linkwarden-logins-api-openapi.yml
  format: yaml
  label: Linkwarden Logins API
  slug: linkwarden-logins-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkwarden/openapi/linkwarden-logins-api-openapi.yml
- filename: linkwarden-migration-api-openapi.yml
  format: yaml
  label: Linkwarden Migration API
  slug: linkwarden-migration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkwarden/openapi/linkwarden-migration-api-openapi.yml
- filename: linkwarden-preserved-api-openapi.yml
  format: yaml
  label: Linkwarden Preserved API
  slug: linkwarden-preserved-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkwarden/openapi/linkwarden-preserved-api-openapi.yml
- filename: linkwarden-public-api-openapi.yml
  format: yaml
  label: Linkwarden Public API
  slug: linkwarden-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkwarden/openapi/linkwarden-public-api-openapi.yml
- filename: linkwarden-rss-api-openapi.yml
  format: yaml
  label: Linkwarden RSS API
  slug: linkwarden-rss-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkwarden/openapi/linkwarden-rss-api-openapi.yml
- filename: linkwarden-search-api-openapi.yml
  format: yaml
  label: Linkwarden Search API
  slug: linkwarden-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkwarden/openapi/linkwarden-search-api-openapi.yml
- filename: linkwarden-session-api-openapi.yml
  format: yaml
  label: Linkwarden Session API
  slug: linkwarden-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkwarden/openapi/linkwarden-session-api-openapi.yml
- filename: linkwarden-tags-api-openapi.yml
  format: yaml
  label: Linkwarden Tags API
  slug: linkwarden-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkwarden/openapi/linkwarden-tags-api-openapi.yml
- filename: linkwarden-tokens-api-openapi.yml
  format: yaml
  label: Linkwarden Tokens API
  slug: linkwarden-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkwarden/openapi/linkwarden-tokens-api-openapi.yml
- filename: linkwarden-users-api-openapi.yml
  format: yaml
  label: Linkwarden Users API
  slug: linkwarden-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkwarden/openapi/linkwarden-users-api-openapi.yml
- filename: linkwarden-worker-api-openapi.yml
  format: yaml
  label: Linkwarden Worker API
  slug: linkwarden-worker-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkwarden/openapi/linkwarden-worker-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Linkwarden Authentication
name_suffix: Authentication
oauth_flows: []
overview: Linkwarden secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Linkwarden
provider_slug: linkwarden
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/linkwarden.yaml
  type: http
slug: linkwarden-authentication
source_filename: linkwarden-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: derived\nsource: openapi/linkwarden.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/linkwarden.yaml\n"
source_yaml_url: https://artifacts.apis.io/linkwarden/authentication/linkwarden-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Bookmarking
- OpenSource
- SelfHostable
- Productivity
---
