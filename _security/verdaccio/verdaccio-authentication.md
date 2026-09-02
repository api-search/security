---
api_key_in: []
api_specs:
- filename: verdaccio-dist-tags-api-openapi.yml
  format: yaml
  label: Verdaccio dist-tags API
  slug: verdaccio-dist-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdaccio/refs/heads/main/openapi/verdaccio-dist-tags-api-openapi.yml
- filename: verdaccio-packages-api-openapi.yml
  format: yaml
  label: Verdaccio packages API
  slug: verdaccio-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdaccio/refs/heads/main/openapi/verdaccio-packages-api-openapi.yml
- filename: verdaccio-profile-api-openapi.yml
  format: yaml
  label: Verdaccio profile API
  slug: verdaccio-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdaccio/refs/heads/main/openapi/verdaccio-profile-api-openapi.yml
- filename: verdaccio-publish-api-openapi.yml
  format: yaml
  label: Verdaccio publish API
  slug: verdaccio-publish-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdaccio/refs/heads/main/openapi/verdaccio-publish-api-openapi.yml
- filename: verdaccio-search-api-openapi.yml
  format: yaml
  label: Verdaccio search API
  slug: verdaccio-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdaccio/refs/heads/main/openapi/verdaccio-search-api-openapi.yml
- filename: verdaccio-tokens-api-openapi.yml
  format: yaml
  label: Verdaccio tokens API
  slug: verdaccio-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdaccio/refs/heads/main/openapi/verdaccio-tokens-api-openapi.yml
- filename: verdaccio-user-api-openapi.yml
  format: yaml
  label: Verdaccio user API
  slug: verdaccio-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdaccio/refs/heads/main/openapi/verdaccio-user-api-openapi.yml
- filename: verdaccio-utility-api-openapi.yml
  format: yaml
  label: Verdaccio utility API
  slug: verdaccio-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdaccio/refs/heads/main/openapi/verdaccio-utility-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Verdaccio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Verdaccio secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Verdaccio
provider_slug: verdaccio
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: JWT token issued by Verdaccio on login
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/verdaccio-npm-registry-api-openapi.yml
  type: http
- description: HTTP Basic Auth with registry username and password
  name: basicAuth
  scheme: basic
  sources:
  - openapi/verdaccio-npm-registry-api-openapi.yml
  type: http
slug: verdaccio-authentication
source_filename: verdaccio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/verdaccio-npm-registry-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token issued by Verdaccio on login\n  sources:\n  - openapi/verdaccio-npm-registry-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth with registry username and password\n  sources:\n  - openapi/verdaccio-npm-registry-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verdaccio/refs/heads/main/authentication/verdaccio-authentication.yml
summary_line: http · 2 schemes
tags:
- npm
- Registry
- Package Manager
- private-registry
- Proxy
- Node.js
- Open-Source
- Self-Hosted
- YARN
- pnpm
- Docker
- Kubernetes
---
