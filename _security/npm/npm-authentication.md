---
anonymous_access: false
api_key_in: []
api_specs:
- filename: npm-registry-api-openapi.yml
  format: yaml
  label: npm Registry API
  slug: registry
  spec_type: OpenAPI
  url: https://artifacts.apis.io/npm/openapi/npm-registry-api-openapi.yml
- filename: npm-hooks-api-openapi.yml
  format: yaml
  label: npm Hooks API
  slug: hooks
  spec_type: OpenAPI
  url: https://artifacts.apis.io/npm/openapi/npm-hooks-api-openapi.yml
- filename: npm-downloads-api-openapi.yml
  format: yaml
  label: npm Downloads API
  slug: npm-downloads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/npm/openapi/npm-downloads-api-openapi.yml
- filename: npm-packages-api-openapi.yml
  format: yaml
  label: npm Packages API
  slug: npm-packages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/npm/openapi/npm-packages-api-openapi.yml
- filename: npm-search-api-openapi.yml
  format: yaml
  label: npm Search API
  slug: npm-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/npm/openapi/npm-search-api-openapi.yml
- filename: npm-trusted-publishers-api-openapi.yml
  format: yaml
  label: npm Trusted Publishers API
  slug: npm-trusted-publishers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/npm/openapi/npm-trusted-publishers-api-openapi.yml
- filename: npm-access-api-openapi.yml
  format: yaml
  label: npm Access API
  slug: npm-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/npm/openapi/npm-access-api-openapi.yml
- filename: npm-audit-api-openapi.yml
  format: yaml
  label: npm Audit API
  slug: npm-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/npm/openapi/npm-audit-api-openapi.yml
- filename: npm-org-api-openapi.yml
  format: yaml
  label: npm Org API
  slug: npm-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/npm/openapi/npm-org-api-openapi.yml
- filename: npm-publish-api-openapi.yml
  format: yaml
  label: npm Publish API
  slug: npm-publish-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/npm/openapi/npm-publish-api-openapi.yml
- filename: npm-stage-api-openapi.yml
  format: yaml
  label: npm Stage API
  slug: npm-stage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/npm/openapi/npm-stage-api-openapi.yml
- filename: npm-team-api-openapi.yml
  format: yaml
  label: npm Team API
  slug: npm-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/npm/openapi/npm-team-api-openapi.yml
- filename: npm-trust-api-openapi.yml
  format: yaml
  label: npm Trust API
  slug: npm-trust-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/npm/openapi/npm-trust-api-openapi.yml
- filename: npm-oidc-api-openapi.yml
  format: yaml
  label: npm OIDC API
  slug: npm-oidc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/npm/openapi/npm-oidc-api-openapi.yml
- filename: npm-tokens-api-openapi.yml
  format: yaml
  label: npm Tokens API
  slug: npm-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/npm/openapi/npm-tokens-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: npm Authentication
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
source_yaml_url: https://artifacts.apis.io/npm/authentication/npm-authentication.yml
summary_line: http · 2 schemes
tags:
- Packages
- JavaScript
- Node.js
- Package Management
- Registry
- Security
- Developer Tools
- npm
---
