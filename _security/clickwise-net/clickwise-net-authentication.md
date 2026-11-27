---
anonymous_access: false
api_key_in:
- cookie
- header
api_specs:
- filename: clickwise-net-account-api-openapi.yml
  format: yaml
  label: Clickwise Account API
  slug: clickwise-net-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-account-api-openapi.yml
- filename: clickwise-net-deals-api-openapi.yml
  format: yaml
  label: Clickwise Deals API
  slug: clickwise-net-deals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-deals-api-openapi.yml
- filename: clickwise-net-feeds-api-openapi.yml
  format: yaml
  label: Clickwise Feeds API
  slug: clickwise-net-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-feeds-api-openapi.yml
- filename: clickwise-net-links-api-openapi.yml
  format: yaml
  label: Clickwise Links API
  slug: clickwise-net-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-links-api-openapi.yml
- filename: clickwise-net-monetize-api-openapi.yml
  format: yaml
  label: Clickwise Monetize API
  slug: clickwise-net-monetize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-monetize-api-openapi.yml
- filename: clickwise-net-news-api-openapi.yml
  format: yaml
  label: Clickwise News API
  slug: clickwise-net-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-news-api-openapi.yml
- filename: clickwise-net-offers-api-openapi.yml
  format: yaml
  label: Clickwise Offers API
  slug: clickwise-net-offers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-offers-api-openapi.yml
- filename: clickwise-net-onboarding-api-openapi.yml
  format: yaml
  label: Clickwise Onboarding API
  slug: clickwise-net-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-onboarding-api-openapi.yml
- filename: clickwise-net-postbacks-api-openapi.yml
  format: yaml
  label: Clickwise Postbacks API
  slug: clickwise-net-postbacks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-postbacks-api-openapi.yml
- filename: clickwise-net-products-api-openapi.yml
  format: yaml
  label: Clickwise Products API
  slug: clickwise-net-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-products-api-openapi.yml
- filename: clickwise-net-programs-api-openapi.yml
  format: yaml
  label: Clickwise Programs API
  slug: clickwise-net-programs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-programs-api-openapi.yml
- filename: clickwise-net-public-api-openapi.yml
  format: yaml
  label: Clickwise Public API
  slug: clickwise-net-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-public-api-openapi.yml
- filename: clickwise-net-reporting-api-openapi.yml
  format: yaml
  label: Clickwise Reporting API
  slug: clickwise-net-reporting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-reporting-api-openapi.yml
- filename: clickwise-net-subscribers-api-openapi.yml
  format: yaml
  label: Clickwise Subscribers API
  slug: clickwise-net-subscribers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-subscribers-api-openapi.yml
- filename: clickwise-net-widgets-api-openapi.yml
  format: yaml
  label: Clickwise Widgets API
  slug: clickwise-net-widgets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-widgets-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Clickwise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clickwise secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Clickwise
provider_slug: clickwise-net
scheme_count: 4
schemes:
- in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/clickwise-net-panel-openapi.yml
  - openapi/clickwise-net-publisher-openapi.yml
  type: apiKey
- in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/clickwise-net-panel-openapi.yml
  type: apiKey
- name: tokenAuth
  scheme: bearer
  sources:
  - openapi/clickwise-net-panel-openapi.yml
  - openapi/clickwise-net-publisher-openapi.yml
  type: http
- applies_to: https://partners.clickwise.net/api/v1/mcp/account
  flows:
  - authorizationCode
  metadata: https://partners.clickwise.net/.well-known/oauth-authorization-server
  name: mcpOAuth
  pkce: S256
  scopes:
  - affiliate:read
  - affiliate:links
  sources:
  - https://partners.clickwise.net/llms-full.txt
  type: oauth2
slug: clickwise-net-authentication
source_filename: clickwise-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- openapi/clickwise-net-panel-openapi.yml, openapi/clickwise-net-publisher-openapi.yml\n- https://partners.clickwise.net/developers/\n- https://partners.clickwise.net/llms-full.txt\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/clickwise-net-panel-openapi.yml\n  - openapi/clickwise-net-publisher-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/clickwise-net-panel-openapi.yml\n- name: tokenAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/clickwise-net-panel-openapi.yml\n  - openapi/clickwise-net-publisher-openapi.yml\n- name: mcpOAuth\n  type: oauth2\n  flows:\n  - authorizationCode\n  pkce: S256\n  scopes:\n  - affiliate:read\n  - affiliate:links\n  applies_to: https://partners.clickwise.net/api/v1/mcp/account\n\
  \  metadata: https://partners.clickwise.net/.well-known/oauth-authorization-server\n  sources:\n  - https://partners.clickwise.net/llms-full.txt\ndocs: https://partners.clickwise.net/llms-full.txt\ncredentials:\n- name: Sandbox key\n  prefix: cw_sbx_\n  works_on: Publisher Products API only plus MCP search_products\n- name: Publisher API key\n  header: 'X-API-Key or Authorization: Bearer'\n  works_on: whole Publisher API v1, MCP account tools, HasOffers/TUNE endpoint\n- name: Reporting API token\n  header: 'Authorization: Bearer'\n  works_on: /api/v1/affiliate-reporting/*\n- name: Offers credential\n  prefix: cw_off_\n  works_on: /offers/ and /offers.csv (pilot)\n- name: Merchant conversions key\n  prefix: cw_mk_\n  header: X-Merchant-Key\n  works_on: POST /api/v1/conversions/\n- name: Site widget public key\n  prefix: cw_pub_\n  works_on: /api/v1/feeds/products/ and widget loader\nnotes: 'Send keys only in the X-API-Key or Authorization: Bearer header, never in URLs, page source or browser\
  \ code.'\n"
source_yaml_url: https://artifacts.apis.io/clickwise-net/authentication/clickwise-net-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- Affiliate Marketing
- Affiliate Network
- Performance Marketing
- tracked-links
- Publishers
- E-Commerce
- MCP
---
