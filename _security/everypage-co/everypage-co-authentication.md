---
anonymous_access: false
api_key_in: []
api_specs:
- filename: everypage-co-account-api-openapi.yml
  format: yaml
  label: EveryPage Account API
  slug: everypage-co-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everypage-co/openapi/everypage-co-account-api-openapi.yml
- filename: everypage-co-embedding-api-openapi.yml
  format: yaml
  label: EveryPage Embedding API
  slug: everypage-co-embedding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everypage-co/openapi/everypage-co-embedding-api-openapi.yml
- filename: everypage-co-events-api-openapi.yml
  format: yaml
  label: EveryPage Events API
  slug: everypage-co-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everypage-co/openapi/everypage-co-events-api-openapi.yml
- filename: everypage-co-files-api-openapi.yml
  format: yaml
  label: EveryPage Files API
  slug: everypage-co-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everypage-co/openapi/everypage-co-files-api-openapi.yml
- filename: everypage-co-oauth-api-openapi.yml
  format: yaml
  label: EveryPage OAuth API
  slug: everypage-co-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everypage-co/openapi/everypage-co-oauth-api-openapi.yml
- filename: everypage-co-variants-api-openapi.yml
  format: yaml
  label: EveryPage Variants API
  slug: everypage-co-variants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everypage-co/openapi/everypage-co-variants-api-openapi.yml
- filename: everypage-co-webhooks-api-openapi.yml
  format: yaml
  label: EveryPage Webhooks API
  slug: everypage-co-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everypage-co/openapi/everypage-co-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: EveryPage Authentication
name_suffix: Authentication
oauth_flows: []
overview: EveryPage declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: EveryPage
provider_slug: everypage-co
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token authentication using API keys (ep_live_) or OAuth access tokens (ep_at_). Include in Authorization header.
  tokenPrefix: ep_live_ or ep_at_
  type: bearer
slug: everypage-co-authentication
source_filename: everypage-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://everypage.co/docs/developers/authentication\nschemes:\n  - type: bearer\n    description: \"Bearer token authentication using API keys (ep_live_) or OAuth access tokens (ep_at_). Include in Authorization header.\"\n    bearerFormat: JWT\n    tokenPrefix: ep_live_ or ep_at_\n"
source_yaml_url: https://artifacts.apis.io/everypage-co/authentication/everypage-co-authentication.yml
summary_line: 1 scheme
tags:
- PDF
- Document Sharing
- ReaderAnalytics
- Privacy
- Software-as-a-Service
---
