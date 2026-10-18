---
anonymous_access: false
api_key_in: []
api_specs:
- filename: voucherify-vouchers-api-openapi.yml
  format: yaml
  label: Voucherify Vouchers API
  slug: voucherify-vouchers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voucherify/refs/heads/main/openapi/voucherify-vouchers-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Voucherify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Voucherify declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Voucherify
provider_slug: voucherify
scheme_count: 5
schemes:
- evidence: 'A generated pair of Application ID and Application Secret Key must be attached to every HTTP request as custom headers: `X-App-Id`, `X-App-Token`.'
  header: X-App-Id
  how_to_obtain: Generate in Project Settings → General → Application Keys
  location: header
  name: Application
  type: apiKey
- evidence: 'A generated pair of Application ID and Application Secret Key must be attached to every HTTP request as custom headers: `X-App-Id`, `X-App-Token`.'
  header: X-App-Token
  how_to_obtain: Generate in Project Settings → General → Application Keys
  location: header
  name: Application
  type: apiKey
- evidence: 'For client-side HTTP requests, you need to provide the following headers:'
  header: X-Client-Application-Id
  how_to_obtain: Generate in Project Settings → General → Client-Side Keys
  location: header
  name: Client-side
  type: apiKey
- evidence: 'For client-side HTTP requests, you need to provide the following headers:'
  header: X-Client-Token
  how_to_obtain: Generate in Project Settings → General → Client-Side Keys
  location: header
  name: Client-side
  type: apiKey
- evidence: Voucherify supports also OAuth 2.0 authorization method.
  flows:
  - client_credentials
  how_to_obtain: Generate using an Application ID and Secret Key via the /v1/oauth/token endpoint
  name: OAuth 2.0
  scopes:
  - api
  - assets
  - async-actions
  - campaigns
  - categories
  - client_api
  - client_consents
  - client_customers
  - client_events
  - client_promotions
  - client_publish
  - client_qualifications
  - client_redeem
  - client_redemptions
  - client_validate
  - client_validations
  - client_vouchers
  - consents
  - customers
  - events
  - exports
  - locations
  - loyalties
  - metadata-schemas
  - orders
  - product-collections
  - products
  - promotions
  - publications
  - qualifications
  - redemptions
  - referrals
  - rewards
  - segments
  - skus
  - task-results
  - templates
  - trash-bin
  - validation-rules-assignments
  - validation-rules
  - validations
  - vouchers
  token_url: https://{cluster}.voucherify.io/v1/oauth/token
  type: oauth2
slug: voucherify-authentication
source_filename: voucherify-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.voucherify.io/guides/authentication.md
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.voucherify.io/guides/authentication.md\nsources:\n- https://docs.voucherify.io/guides/authentication.md\n- https://docs.voucherify.io/api-reference/oauth/generate-oauth-20-token.md\n- https://docs.voucherify.io/api-reference/oauth/introspect-oauth-20-token.md\n- https://docs.voucherify.io/api-reference/oauth/revoke-oauth-20-token.md\nschemes:\n- type: apiKey\n  name: Application\n  evidence: 'A generated pair of Application ID and Application Secret Key must be attached to every HTTP request as custom headers: `X-App-Id`,\n    `X-App-Token`.'\n  location: header\n  header: X-App-Id\n  how_to_obtain: Generate in Project Settings → General → Application Keys\n- type: apiKey\n  name: Application\n  evidence: 'A generated pair of Application ID and Application Secret Key must be attached to every HTTP request as custom headers: `X-App-Id`,\n    `X-App-Token`.'\n  location:\
  \ header\n  header: X-App-Token\n  how_to_obtain: Generate in Project Settings → General → Application Keys\n- type: apiKey\n  name: Client-side\n  evidence: 'For client-side HTTP requests, you need to provide the following headers:'\n  location: header\n  header: X-Client-Application-Id\n  how_to_obtain: Generate in Project Settings → General → Client-Side Keys\n- type: apiKey\n  name: Client-side\n  evidence: 'For client-side HTTP requests, you need to provide the following headers:'\n  location: header\n  header: X-Client-Token\n  how_to_obtain: Generate in Project Settings → General → Client-Side Keys\n- type: oauth2\n  name: OAuth 2.0\n  evidence: Voucherify supports also OAuth 2.0 authorization method.\n  flows:\n  - client_credentials\n  token_url: https://{cluster}.voucherify.io/v1/oauth/token\n  scopes:\n  - api\n  - assets\n  - async-actions\n  - campaigns\n  - categories\n  - client_api\n  - client_consents\n  - client_customers\n  - client_events\n  - client_promotions\n  -\
  \ client_publish\n  - client_qualifications\n  - client_redeem\n  - client_redemptions\n  - client_validate\n  - client_validations\n  - client_vouchers\n  - consents\n  - customers\n  - events\n  - exports\n  - locations\n  - loyalties\n  - metadata-schemas\n  - orders\n  - product-collections\n  - products\n  - promotions\n  - publications\n  - qualifications\n  - redemptions\n  - referrals\n  - rewards\n  - segments\n  - skus\n  - task-results\n  - templates\n  - trash-bin\n  - validation-rules-assignments\n  - validation-rules\n  - validations\n  - vouchers\n  how_to_obtain: Generate using an Application ID and Secret Key via the /v1/oauth/token endpoint\ndocs: https://docs.voucherify.io/guides/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voucherify/refs/heads/main/authentication/voucherify-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Incentives
- Promotions
- Loyalty
---
