---
api_key_in:
- header
api_specs:
- filename: tapfiliate-affiliate-groups-api-openapi.yml
  format: yaml
  label: Tapfiliate Affiliate Groups API
  slug: tapfiliate-affiliate-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-affiliate-groups-api-openapi.yml
- filename: tapfiliate-affiliate-prospects-api-openapi.yml
  format: yaml
  label: Tapfiliate Affiliate Prospects API
  slug: tapfiliate-affiliate-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-affiliate-prospects-api-openapi.yml
- filename: tapfiliate-affiliates-api-openapi.yml
  format: yaml
  label: Tapfiliate Affiliates API
  slug: tapfiliate-affiliates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-affiliates-api-openapi.yml
- filename: tapfiliate-balances-api-openapi.yml
  format: yaml
  label: Tapfiliate Balances API
  slug: tapfiliate-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-balances-api-openapi.yml
- filename: tapfiliate-clicks-api-openapi.yml
  format: yaml
  label: Tapfiliate Clicks API
  slug: tapfiliate-clicks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-clicks-api-openapi.yml
- filename: tapfiliate-commissions-api-openapi.yml
  format: yaml
  label: Tapfiliate Commissions API
  slug: tapfiliate-commissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-commissions-api-openapi.yml
- filename: tapfiliate-conversions-api-openapi.yml
  format: yaml
  label: Tapfiliate Conversions API
  slug: tapfiliate-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-conversions-api-openapi.yml
- filename: tapfiliate-customers-api-openapi.yml
  format: yaml
  label: Tapfiliate Customers API
  slug: tapfiliate-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-customers-api-openapi.yml
- filename: tapfiliate-payments-api-openapi.yml
  format: yaml
  label: Tapfiliate Payments API
  slug: tapfiliate-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-payments-api-openapi.yml
- filename: tapfiliate-programs-api-openapi.yml
  format: yaml
  label: Tapfiliate Programs API
  slug: tapfiliate-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-programs-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: Tapfiliate has two authentication surfaces that do not share a mechanism. The REST API v1.6 uses a single static account API key sent as a request header — no OAuth, no token exchange, no per-integration scoping, and the key can approve commissions and create payments. The MCP server, announced 2026-08-07, is a proper OAuth 2.0 protected resource with PKCE, dynamic client registration and four declared scopes.
kind: authentication
layout: security
method: searched
name: Tapfiliate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tapfiliate secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tapfiliate
provider_slug: tapfiliate
scheme_count: 2
schemes:
- applies_to: https://api.tapfiliate.com/1.6
  in: header
  key_management: Account settings / profile settings in the Tapfiliate dashboard.
  name: ApiKeyAuth
  note: The reference documents the header as `X-Api-Key`. The REST integration guide at /docs/integrations/rest-api/ shows curl examples using a bare `Api-Key:` header instead, and the trigger-webhook guide also says to set "your Api-Key in the header field". Recorded as observed; `X-Api-Key` is the form both the reference and the OpenAPI carry.
  parameter: X-Api-Key
  rotation: No documented rotation policy, expiry or key-prefix convention.
  scoping: None. One account-level key carries the full surface. Tapfiliate's own docs warn the key can approve commissions and must never be exposed in frontend javascript or public repositories.
  sources:
  - openapi/tapfiliate-affiliate-groups-api-openapi.yml
  - openapi/tapfiliate-affiliate-prospects-api-openapi.yml
  - openapi/tapfiliate-affiliates-api-openapi.yml
  - openapi/tapfiliate-balances-api-openapi.yml
  - openapi/tapfiliate-clicks-api-openapi.yml
  - openapi/tapfiliate-commissions-api-openapi.yml
  - openapi/tapfiliate-conversions-api-openapi.yml
  - openapi/tapfiliate-customers-api-openapi.yml
  - openapi/tapfiliate-payments-api-openapi.yml
  - openapi/tapfiliate-programs-api-openapi.yml
  - https://tapfiliate.com/docs/rest/#header-authentication
  transport: HTTPS only — plain HTTP calls fail, and unauthenticated requests fail.
  type: apiKey
- applies_to: https://mcp.tapfiliate.com/mcp
  bearer_methods:
  - header
  detail: scopes/tapfiliate-scopes.yml
  dynamic_client_registration: https://app.tapfiliate.com/oauth/v2/register/
  flows:
    authorizationCode:
      authorizationUrl: https://app.tapfiliate.com/ai/mcp/connect/
      refreshUrl: https://mcp.tapfiliate.com/oauth/v2/token/
      scopes:
        affiliates: Affiliates, affiliate groups and affiliate prospects
        conversions_commissions: Clicks, customers, conversions and commissions
        payments: Affiliate balances and payouts
        programs: Affiliate programs, commission types, MLM levels and bonuses
      tokenUrl: https://mcp.tapfiliate.com/oauth/v2/token/
  issuer: https://api.tapfiliate.com
  jwks_uri: https://api.tapfiliate.com/.well-known/jwks.json
  name: TapfiliateMcpOAuth
  pkce:
  - S256
  prerequisites:
  - Admin-level Tapfiliate account permissions
  - API/Zapier access enabled on the account
  sources:
  - https://mcp.tapfiliate.com/.well-known/oauth-authorization-server
  - https://mcp.tapfiliate.com/.well-known/oauth-protected-resource
  - https://support.tapfiliate.com/en/articles/16011230-how-to-use-your-new-affiliate-analyst-the-tapfiliate-mcp-server
  type: oauth2
slug: tapfiliate-authentication
source_filename: tapfiliate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://tapfiliate.com/docs/rest/#header-authentication (REST reference),\n  https://tapfiliate.com/docs/integrations/rest-api/ (integration guide),\n  https://mcp.tapfiliate.com/.well-known/oauth-authorization-server (live probe,\n  HTTP 200), and the securitySchemes in openapi/.\ndocs: https://tapfiliate.com/docs/rest/#header-authentication\ndescription: >-\n  Tapfiliate has two authentication surfaces that do not share a mechanism. The\n  REST API v1.6 uses a single static account API key sent as a request header —\n  no OAuth, no token exchange, no per-integration scoping, and the key can\n  approve commissions and create payments. The MCP server, announced 2026-08-07,\n  is a proper OAuth 2.0 protected resource with PKCE, dynamic client\n  registration and four declared scopes.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter:\
  \ X-Api-Key\n  applies_to: https://api.tapfiliate.com/1.6\n  transport: HTTPS only — plain HTTP calls fail, and unauthenticated requests fail.\n  key_management: Account settings / profile settings in the Tapfiliate dashboard.\n  rotation: No documented rotation policy, expiry or key-prefix convention.\n  scoping: >-\n    None. One account-level key carries the full surface. Tapfiliate's own docs\n    warn the key can approve commissions and must never be exposed in frontend\n    javascript or public repositories.\n  sources:\n  - openapi/tapfiliate-affiliate-groups-api-openapi.yml\n  - openapi/tapfiliate-affiliate-prospects-api-openapi.yml\n  - openapi/tapfiliate-affiliates-api-openapi.yml\n  - openapi/tapfiliate-balances-api-openapi.yml\n  - openapi/tapfiliate-clicks-api-openapi.yml\n  - openapi/tapfiliate-commissions-api-openapi.yml\n  - openapi/tapfiliate-conversions-api-openapi.yml\n  - openapi/tapfiliate-customers-api-openapi.yml\n  - openapi/tapfiliate-payments-api-openapi.yml\n\
  \  - openapi/tapfiliate-programs-api-openapi.yml\n  - https://tapfiliate.com/docs/rest/#header-authentication\n  note: >-\n    The reference documents the header as `X-Api-Key`. The REST integration guide\n    at /docs/integrations/rest-api/ shows curl examples using a bare `Api-Key:`\n    header instead, and the trigger-webhook guide also says to set \"your Api-Key\n    in the header field\". Recorded as observed; `X-Api-Key` is the form both the\n    reference and the OpenAPI carry.\n- name: TapfiliateMcpOAuth\n  type: oauth2\n  applies_to: https://mcp.tapfiliate.com/mcp\n  flows:\n    authorizationCode:\n      authorizationUrl: https://app.tapfiliate.com/ai/mcp/connect/\n      tokenUrl: https://mcp.tapfiliate.com/oauth/v2/token/\n      refreshUrl: https://mcp.tapfiliate.com/oauth/v2/token/\n      scopes:\n        affiliates: Affiliates, affiliate groups and affiliate prospects\n        conversions_commissions: Clicks, customers, conversions and commissions\n        programs: Affiliate\
  \ programs, commission types, MLM levels and bonuses\n        payments: Affiliate balances and payouts\n  issuer: https://api.tapfiliate.com\n  jwks_uri: https://api.tapfiliate.com/.well-known/jwks.json\n  pkce: [S256]\n  dynamic_client_registration: https://app.tapfiliate.com/oauth/v2/register/\n  bearer_methods: [header]\n  prerequisites:\n  - Admin-level Tapfiliate account permissions\n  - API/Zapier access enabled on the account\n  detail: scopes/tapfiliate-scopes.yml\n  sources:\n  - https://mcp.tapfiliate.com/.well-known/oauth-authorization-server\n  - https://mcp.tapfiliate.com/.well-known/oauth-protected-resource\n  - https://support.tapfiliate.com/en/articles/16011230-how-to-use-your-new-affiliate-analyst-the-tapfiliate-mcp-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/authentication/tapfiliate-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Affiliate Marketing
- Affiliate Tracking
- Commission Management
- Conversion Tracking
- Partner Programs
- Referral Programs
- Influencer Marketing
---
