---
api_key_in:
- header
api_specs:
- filename: goody-brands-api-openapi.yml
  format: yaml
  label: Goody Brands API
  slug: goody-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-brands-api-openapi.yml
- filename: goody-cards-api-openapi.yml
  format: yaml
  label: Goody Cards API
  slug: goody-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-cards-api-openapi.yml
- filename: goody-collections-api-openapi.yml
  format: yaml
  label: Goody Collections API
  slug: goody-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-collections-api-openapi.yml
- filename: goody-commerce-user-payment-methods-api-openapi.yml
  format: yaml
  label: Goody Commerce User Payment Methods API
  slug: goody-commerce-user-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-commerce-user-payment-methods-api-openapi.yml
- filename: goody-me-api-openapi.yml
  format: yaml
  label: Goody Me API
  slug: goody-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-me-api-openapi.yml
- filename: goody-order-activities-api-openapi.yml
  format: yaml
  label: Goody Order Activities API
  slug: goody-order-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-order-activities-api-openapi.yml
- filename: goody-order-batches-api-openapi.yml
  format: yaml
  label: Goody Order Batches API
  slug: goody-order-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-order-batches-api-openapi.yml
- filename: goody-orders-api-openapi.yml
  format: yaml
  label: Goody Orders API
  slug: goody-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-orders-api-openapi.yml
- filename: goody-payment-methods-api-openapi.yml
  format: yaml
  label: Goody Payment Methods API
  slug: goody-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-payment-methods-api-openapi.yml
- filename: goody-products-api-openapi.yml
  format: yaml
  label: Goody Products API
  slug: goody-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-products-api-openapi.yml
- filename: goody-webhooks-api-openapi.yml
  format: yaml
  label: Goody Webhooks API
  slug: goody-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-webhooks-api-openapi.yml
- filename: goody-workspaces-api-openapi.yml
  format: yaml
  label: Goody Workspaces API
  slug: goody-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-workspaces-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Goody Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Goody secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Goody
provider_slug: goody
scheme_count: 2
schemes:
- description: 'Goody API key (Commerce API / Automation API). Passed as "Authorization: Bearer [example key]". Production and Sandbox accounts are separate and carry different keys for isolation.'
  docs: https://developer.ongoody.com/commerce-api/authentication
  name: bearer
  scheme: bearer
  sources:
  - openapi/goody-api-openapi-original.json
  type: http
- description: OAuth 2.0 authorization-code + PKCE (S256) used by the Goody MCP server for interactive clients (Claude, Cursor). Supports dynamic client registration (RFC 7591). Advertised at /.well-known/oauth-authorization-server (RFC 8414). Scripts/automations may instead pass a personal MCP token as a bearer token.
  docs: https://developer.ongoody.com/mcp/authentication
  flows:
  - authorizationUrl: https://api.ongoody.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://api.ongoody.com/oauth/register
    revocationUrl: https://api.ongoody.com/oauth/revoke
    scopes:
    - mcp.read
    - mcp.write
    - mcp.gifts
    - chrome.write
    tokenUrl: https://api.ongoody.com/oauth/token
  name: mcp_oauth2
  sources:
  - well-known/goody-oauth-authorization-server.json
  type: oauth2
slug: goody-authentication
source_filename: goody-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/goody-api-openapi-original.json\ndocs: https://developer.ongoody.com/commerce-api/authentication\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: >-\n    Goody API key (Commerce API / Automation API). Passed as\n    \"Authorization: Bearer [example key]\". Production and Sandbox\n    accounts are separate and carry different keys for isolation.\n  docs: https://developer.ongoody.com/commerce-api/authentication\n  sources:\n  - openapi/goody-api-openapi-original.json\n- name: mcp_oauth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization-code + PKCE (S256) used by the Goody MCP server\n    for interactive clients (Claude, Cursor). Supports dynamic client\n    registration (RFC 7591). Advertised at\n    /.well-known/oauth-authorization-server (RFC 8414). Scripts/automations\n\
  \    may instead pass a personal MCP token as a bearer token.\n  docs: https://developer.ongoody.com/mcp/authentication\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.ongoody.com/oauth/authorize\n    tokenUrl: https://api.ongoody.com/oauth/token\n    registrationUrl: https://api.ongoody.com/oauth/register\n    revocationUrl: https://api.ongoody.com/oauth/revoke\n    pkce: S256\n    scopes:\n    - mcp.read\n    - mcp.write\n    - mcp.gifts\n    - chrome.write\n  sources:\n  - well-known/goody-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/authentication/goody-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Retail
- Gifting
- Gift Cards
- E-Commerce
- Commerce
- Payments
- MCP
- Webhooks
- Rewards
---
