---
api_key_in: []
api_specs:
- filename: npm-registry-api-openapi.yml
  format: yaml
  label: npm Registry API
  slug: registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/npm/refs/heads/main/openapi/npm-registry-api-openapi.yml
- filename: npm-hooks-api-openapi.yml
  format: yaml
  label: npm Hooks API
  slug: hooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/npm/refs/heads/main/openapi/npm-hooks-api-openapi.yml
- filename: npm-downloads-api-openapi.yml
  format: yaml
  label: npm Downloads API
  slug: npm-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/npm/refs/heads/main/openapi/npm-downloads-api-openapi.yml
- filename: npm-oidc-api-openapi.yml
  format: yaml
  label: npm OIDC API
  slug: npm-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/npm/refs/heads/main/openapi/npm-oidc-api-openapi.yml
- filename: npm-packages-api-openapi.yml
  format: yaml
  label: npm Packages API
  slug: npm-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/npm/refs/heads/main/openapi/npm-packages-api-openapi.yml
- filename: npm-search-api-openapi.yml
  format: yaml
  label: npm Search API
  slug: npm-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/npm/refs/heads/main/openapi/npm-search-api-openapi.yml
- filename: npm-tokens-api-openapi.yml
  format: yaml
  label: npm Tokens API
  slug: npm-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/npm/refs/heads/main/openapi/npm-tokens-api-openapi.yml
- filename: npm-trusted-publishers-api-openapi.yml
  format: yaml
  label: npm Trusted Publishers API
  slug: npm-trusted-publishers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/npm/refs/heads/main/openapi/npm-trusted-publishers-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Npm Authentication
name_suffix: Authentication
oauth_flows: []
overview: npm secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: npm
provider_slug: npm
scheme_count: 2
schemes:
- description: npm access token provided as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/npm-hooks-api-openapi.yml
  - openapi/npm-public-api-openapi.yml
  type: http
- description: Basic authentication using npm username and password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/npm-public-api-openapi.yml
  type: http
slug: npm-authentication
source_filename: npm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/npm-hooks-api-openapi.yml, openapi/npm-public-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: npm access token provided as a Bearer token.\n  sources:\n  - openapi/npm-hooks-api-openapi.yml\n  - openapi/npm-public-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication using npm username and password.\n  sources:\n  - openapi/npm-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/npm/refs/heads/main/authentication/npm-authentication.yml
summary_line: http · 2 schemes
tags:
- Packages
- JavaScript
- Node.js
- Package Management
- Registry
- Security
---
