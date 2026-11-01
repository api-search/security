---
anonymous_access: false
api_key_in: []
api_specs:
- filename: signalaf-com-hall-api-openapi.yml
  format: yaml
  label: signalaf-com Hall API
  slug: signalaf-com-hall-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signalaf-com/openapi/signalaf-com-hall-api-openapi.yml
- filename: signalaf-com-leaderboard-api-openapi.yml
  format: yaml
  label: signalaf-com Leaderboard API
  slug: signalaf-com-leaderboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signalaf-com/openapi/signalaf-com-leaderboard-api-openapi.yml
- filename: signalaf-com-metrics-api-openapi.yml
  format: yaml
  label: signalaf-com Metrics API
  slug: signalaf-com-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signalaf-com/openapi/signalaf-com-metrics-api-openapi.yml
- filename: signalaf-com-operators-api-openapi.yml
  format: yaml
  label: signalaf-com Operators API
  slug: signalaf-com-operators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signalaf-com/openapi/signalaf-com-operators-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Signalaf Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: signalaf-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: signalaf-com
provider_slug: signalaf-com
scheme_count: 1
schemes:
- authorizationUrl: https://copqtaqzsdvpdbhpwjmt.supabase.co/auth/v1/oauth/authorize
  description: OAuth 2.0 Authorization Code flow via Supabase Auth
  flow: authorization_code
  scopes:
    email: User email address
    offline_access: Refresh token access
    openid: OpenID Connect identifier
    profile: User profile information
  tokenUrl: https://copqtaqzsdvpdbhpwjmt.supabase.co/auth/v1/oauth/token
  type: oauth2
slug: signalaf-com-authentication
source_filename: signalaf-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: \"https://signalaf.com/auth.md\"\nschemes:\n  - type: oauth2\n    flow: authorization_code\n    authorizationUrl: https://copqtaqzsdvpdbhpwjmt.supabase.co/auth/v1/oauth/authorize\n    tokenUrl: https://copqtaqzsdvpdbhpwjmt.supabase.co/auth/v1/oauth/token\n    scopes:\n      openid: \"OpenID Connect identifier\"\n      profile: \"User profile information\"\n      email: \"User email address\"\n      offline_access: \"Refresh token access\"\n    description: \"OAuth 2.0 Authorization Code flow via Supabase Auth\"\n"
source_yaml_url: https://artifacts.apis.io/signalaf-com/authentication/signalaf-com-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Analytics
- Leaderboard
- OpenAPI
- PublicAPI
---
