---
anonymous_access: false
api_key_in: []
api_specs:
- filename: xauconnect-com-analytics-api-openapi.yml
  format: yaml
  label: XAUConnect Analytics API
  slug: xauconnect-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xauconnect-com/openapi/xauconnect-com-analytics-api-openapi.yml
- filename: xauconnect-com-cross-chain-api-openapi.yml
  format: yaml
  label: XAUConnect Cross Chain API
  slug: xauconnect-com-cross-chain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xauconnect-com/openapi/xauconnect-com-cross-chain-api-openapi.yml
- filename: xauconnect-com-meta-api-openapi.yml
  format: yaml
  label: XAUConnect Meta API
  slug: xauconnect-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xauconnect-com/openapi/xauconnect-com-meta-api-openapi.yml
- filename: xauconnect-com-swap-api-openapi.yml
  format: yaml
  label: XAUConnect Swap API
  slug: xauconnect-com-swap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xauconnect-com/openapi/xauconnect-com-swap-api-openapi.yml
auth_types: []
description: Optional wallet JWT POST /auth/challenge → sign message → POST /auth/verify for profile and admin access.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: XAUConnect Authentication
name_suffix: Authentication
oauth_flows: []
overview: XAUConnect declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: XAUConnect
provider_slug: xauconnect-com
scheme_count: 1
schemes:
- evidence: Optional wallet JWT POST /auth/challenge → sign message → POST /auth/verify for profile and admin access.
  header: Authorization
  location: header
  name: JWT
  type: http-bearer
slug: xauconnect-com-authentication
source_filename: xauconnect-com-authentication.yml
source_heading: Authentication Profile
source_url: https://xauconnect.com/developers/api/authentication
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://xauconnect.com/developers/api/authentication\nsources:\n- https://xauconnect.com/developers/api/authentication\n- https://xauconnect.com/learn/guides/how-to-launch-a-token-on-xauconnect\n- https://xauconnect.com/learn/guides/how-to-swap-tokens-on-xauconnect\n- https://xauconnect.com/developers/quickstart\ndescription: Optional wallet JWT POST /auth/challenge → sign message → POST /auth/verify for profile and admin access.\nschemes:\n- type: http-bearer\n  name: JWT\n  evidence: Optional wallet JWT POST /auth/challenge → sign message → POST /auth/verify for profile and admin access.\n  location: header\n  header: Authorization\ndocs: https://xauconnect.com/developers/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/xauconnect-com/authentication/xauconnect-com-authentication.yml
summary_line: 1 scheme
tags:
- Fintech
- DeFi
- Blockchain
- Token Launch
- Solana
---
