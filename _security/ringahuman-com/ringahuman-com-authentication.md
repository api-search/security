---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ringahuman-com-openapi-generated.yml
  format: yaml
  label: ringahuman-com API
  slug: ringahuman-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ringahuman-com/openapi/_ae-authored/ringahuman-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ringahuman Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: ringahuman-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ringahuman-com
provider_slug: ringahuman-com
scheme_count: 2
schemes:
- description: 'Bearer token, e.g., Authorization: Bearer rah_live_...'
  in: header
  name: Authorization
  type: apiKey
- authorizationUrl: https://ringahuman.com/.well-known/oauth-authorization-server/authorize
  description: OAuth 2.1 Authorization Code with PKCE for apps.
  flow: authorizationCode
  scopes:
  - calls
  tokenUrl: https://ringahuman.com/.well-known/oauth-authorization-server/token
  type: oauth2
slug: ringahuman-com-authentication
source_filename: ringahuman-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://ringahuman.com/docs/authentication/\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Bearer token, e.g., Authorization: Bearer rah_live_...\"\n  - type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://ringahuman.com/.well-known/oauth-authorization-server/authorize\n    tokenUrl: https://ringahuman.com/.well-known/oauth-authorization-server/token\n    scopes:\n      - calls\n    description: \"OAuth 2.1 Authorization Code with PKCE for apps.\"\n"
source_yaml_url: https://artifacts.apis.io/ringahuman-com/authentication/ringahuman-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Telephony
- LeadGeneration
- Compliance
---
