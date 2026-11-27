---
anonymous_access: false
api_key_in: []
api_specs:
- filename: loyaltyvip-com-account-api-openapi.yml
  format: yaml
  label: LoyaltyVIP Account API
  slug: loyaltyvip-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loyaltyvip-com/openapi/loyaltyvip-com-account-api-openapi.yml
- filename: loyaltyvip-com-directory-api-openapi.yml
  format: yaml
  label: LoyaltyVIP Directory API
  slug: loyaltyvip-com-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loyaltyvip-com/openapi/loyaltyvip-com-directory-api-openapi.yml
- filename: loyaltyvip-com-features-api-openapi.yml
  format: yaml
  label: LoyaltyVIP Features API
  slug: loyaltyvip-com-features-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loyaltyvip-com/openapi/loyaltyvip-com-features-api-openapi.yml
- filename: loyaltyvip-com-player-api-api-openapi.yml
  format: yaml
  label: LoyaltyVIP Player API
  slug: loyaltyvip-com-player-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loyaltyvip-com/openapi/loyaltyvip-com-player-api-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: LoyaltyVIP Authentication
name_suffix: Authentication
oauth_flows: []
overview: LoyaltyVIP secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LoyaltyVIP
provider_slug: loyaltyvip-com
scheme_count: 1
schemes:
- bearerFormat: lvip_live_*
  description: 'Personal API key as a Bearer token. Scopes: read, write, tax, host. Create at https://loyaltyvip.com/dashboard/developer.'
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/loyaltyvip-com-openapi.yml
  type: http
slug: loyaltyvip-com-authentication
source_filename: loyaltyvip-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/loyaltyvip-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: lvip_live_*\n  description: 'Personal API key as a Bearer token. Scopes: read, write, tax, host. Create at\n    https://loyaltyvip.com/dashboard/developer.'\n  sources:\n  - openapi/loyaltyvip-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/loyaltyvip-com/authentication/loyaltyvip-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Casinos
- Player Intelligence
- Loyalty
- Data Analytics
- Gaming
---
