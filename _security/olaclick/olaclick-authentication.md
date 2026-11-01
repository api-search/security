---
anonymous_access: false
api_key_in: []
api_specs:
- filename: olaclick-openapi-generated.yml
  format: yaml
  label: OlaClick API
  slug: olaclick-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/olaclick/openapi/_ae-authored/olaclick-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Olaclick Authentication
name_suffix: Authentication
oauth_flows: []
overview: OlaClick declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: OlaClick
provider_slug: olaclick
scheme_count: 2
schemes:
- description: Obtain access tokens using API Key (client ID) and secret.
  flow: client_credentials
  tokenUrl: https://api.olaclick.com/oauth/token
  type: oauth2
- description: Static API keys for simple authentication.
  in: header
  name: X-API-Key
  type: apiKey
slug: olaclick-authentication
source_filename: olaclick-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://developers.olaclick.app/docs/authentication/api-keys\nschemes:\n  - type: oauth2\n    flow: client_credentials\n    tokenUrl: https://api.olaclick.com/oauth/token\n    description: Obtain access tokens using API Key (client ID) and secret.\n  - type: apiKey\n    in: header\n    name: X-API-Key\n    description: Static API keys for simple authentication.\n"
source_yaml_url: https://artifacts.apis.io/olaclick/authentication/olaclick-authentication.yml
summary_line: 2 schemes
tags:
- Restaurant
- POS
- AI
- SaaS
- Delivery
---
