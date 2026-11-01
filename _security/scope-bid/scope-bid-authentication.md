---
anonymous_access: false
api_key_in: []
api_specs:
- filename: scope-bid-carrier-feed-api-openapi.yml
  format: yaml
  label: scope-bid Carrier Feed API
  slug: scope-bid-carrier-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-carrier-feed-api-openapi.yml
- filename: scope-bid-deliverables-api-openapi.yml
  format: yaml
  label: scope-bid Deliverables API
  slug: scope-bid-deliverables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-deliverables-api-openapi.yml
- filename: scope-bid-dispatches-api-openapi.yml
  format: yaml
  label: scope-bid Dispatches API
  slug: scope-bid-dispatches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-dispatches-api-openapi.yml
- filename: scope-bid-exports-api-openapi.yml
  format: yaml
  label: scope-bid Exports API
  slug: scope-bid-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-exports-api-openapi.yml
- filename: scope-bid-insights-api-openapi.yml
  format: yaml
  label: scope-bid Insights API
  slug: scope-bid-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-insights-api-openapi.yml
- filename: scope-bid-matters-api-openapi.yml
  format: yaml
  label: scope-bid Matters API
  slug: scope-bid-matters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-matters-api-openapi.yml
- filename: scope-bid-partner-authorizations-api-openapi.yml
  format: yaml
  label: scope-bid Partner Authorizations API
  slug: scope-bid-partner-authorizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-partner-authorizations-api-openapi.yml
- filename: scope-bid-scopes-api-openapi.yml
  format: yaml
  label: scope-bid Scopes API
  slug: scope-bid-scopes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-scopes-api-openapi.yml
- filename: scope-bid-vendors-api-openapi.yml
  format: yaml
  label: scope-bid Vendors API
  slug: scope-bid-vendors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-vendors-api-openapi.yml
- filename: scope-bid-webhooks-api-openapi.yml
  format: yaml
  label: scope-bid Webhooks API
  slug: scope-bid-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Scope Bid Authentication
name_suffix: Authentication
oauth_flows: []
overview: scope-bid secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: scope-bid
provider_slug: scope-bid
scheme_count: 1
schemes:
- description: 'OAuth 2.0 access token, or a personal access token (PAT) for CI and power users. Pass as Authorization: Bearer <token>. Every token resolves to exactly one tenant.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/scope-bid-openapi.json
  type: http
slug: scope-bid-authentication
source_filename: scope-bid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/scope-bid-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'OAuth 2.0 access token, or a personal access token (PAT) for CI and power users.\n    Pass as Authorization: Bearer <token>. Every token resolves to exactly one tenant.'\n  sources:\n  - openapi/scope-bid-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/scope-bid/authentication/scope-bid-authentication.yml
summary_line: http · 1 scheme
tags:
- Construction
- Bidding
- SaaS
- Collaboration
- Analytics
---
