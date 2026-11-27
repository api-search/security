---
anonymous_access: false
api_key_in: []
api_specs:
- filename: everpop-app-campaigns-api-openapi.yml
  format: yaml
  label: Everpop Campaigns API
  slug: everpop-app-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everpop-app/openapi/everpop-app-campaigns-api-openapi.yml
- filename: everpop-app-clip-api-openapi.yml
  format: yaml
  label: Everpop Clip API
  slug: everpop-app-clip-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everpop-app/openapi/everpop-app-clip-api-openapi.yml
- filename: everpop-app-generate-api-openapi.yml
  format: yaml
  label: Everpop Generate API
  slug: everpop-app-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everpop-app/openapi/everpop-app-generate-api-openapi.yml
- filename: everpop-app-jobs-api-openapi.yml
  format: yaml
  label: Everpop Jobs API
  slug: everpop-app-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everpop-app/openapi/everpop-app-jobs-api-openapi.yml
- filename: everpop-app-posts-api-openapi.yml
  format: yaml
  label: Everpop Posts API
  slug: everpop-app-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everpop-app/openapi/everpop-app-posts-api-openapi.yml
- filename: everpop-app-publish-api-openapi.yml
  format: yaml
  label: Everpop Publish API
  slug: everpop-app-publish-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everpop-app/openapi/everpop-app-publish-api-openapi.yml
- filename: everpop-app-receipts-api-openapi.yml
  format: yaml
  label: Everpop Receipts API
  slug: everpop-app-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everpop-app/openapi/everpop-app-receipts-api-openapi.yml
- filename: everpop-app-usage-api-openapi.yml
  format: yaml
  label: Everpop Usage API
  slug: everpop-app-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everpop-app/openapi/everpop-app-usage-api-openapi.yml
- filename: everpop-app-videos-api-openapi.yml
  format: yaml
  label: Everpop Videos API
  slug: everpop-app-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everpop-app/openapi/everpop-app-videos-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Everpop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Everpop declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Everpop
provider_slug: everpop-app
scheme_count: 2
schemes:
- description: 'Bearer epk_... API key provided by user via dashboard. Sent as Authorization: Bearer <key>.'
  in: header
  name: Authorization
  type: apiKey
- description: OAuth 2.1 with PKCE (S256). Discovery at /.well-known/oauth-authorization-server. Public clients only. Dynamic client registration is open at the registration_endpoint.
  flows:
    authorizationCode:
      authorizationUrl: https://everpop.app/.well-known/oauth-authorization-server
      scopes: {}
      tokenUrl: https://everpop.app/.well-known/oauth-authorization-server/token
  type: oauth2
slug: everpop-app-authentication
source_filename: everpop-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://everpop.app/auth.md\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Bearer epk_... API key provided by user via dashboard. Sent as Authorization: Bearer <key>.\"\n  - type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://everpop.app/.well-known/oauth-authorization-server\n        tokenUrl: https://everpop.app/.well-known/oauth-authorization-server/token\n        scopes: {}\n    description: \"OAuth 2.1 with PKCE (S256). Discovery at /.well-known/oauth-authorization-server. Public clients only. Dynamic client registration is open at the registration_endpoint.\"\n"
source_yaml_url: https://artifacts.apis.io/everpop-app/authentication/everpop-app-authentication.yml
summary_line: 2 schemes
tags:
- Video
- Artificial Intelligence
- Social Media
- Shorts
- Reels
---
