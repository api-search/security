---
anonymous_access: false
api_key_in: []
api_specs:
- filename: esimker-com-account-api-openapi.yml
  format: yaml
  label: esimker Account API
  slug: esimker-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esimker-com/openapi/esimker-com-account-api-openapi.yml
- filename: esimker-com-blog-api-openapi.yml
  format: yaml
  label: esimker Blog API
  slug: esimker-com-blog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esimker-com/openapi/esimker-com-blog-api-openapi.yml
- filename: esimker-com-catalog-api-openapi.yml
  format: yaml
  label: esimker Catalog API
  slug: esimker-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esimker-com/openapi/esimker-com-catalog-api-openapi.yml
- filename: esimker-com-orders-api-openapi.yml
  format: yaml
  label: esimker Orders API
  slug: esimker-com-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esimker-com/openapi/esimker-com-orders-api-openapi.yml
- filename: esimker-com-pages-api-openapi.yml
  format: yaml
  label: esimker Pages API
  slug: esimker-com-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esimker-com/openapi/esimker-com-pages-api-openapi.yml
- filename: esimker-com-rates-api-openapi.yml
  format: yaml
  label: esimker Rates API
  slug: esimker-com-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esimker-com/openapi/esimker-com-rates-api-openapi.yml
- filename: esimker-com-reseller-api-openapi.yml
  format: yaml
  label: esimker Reseller API
  slug: esimker-com-reseller-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esimker-com/openapi/esimker-com-reseller-api-openapi.yml
- filename: esimker-com-seo-api-openapi.yml
  format: yaml
  label: esimker Seo API
  slug: esimker-com-seo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esimker-com/openapi/esimker-com-seo-api-openapi.yml
- filename: esimker-com-support-api-openapi.yml
  format: yaml
  label: esimker Support API
  slug: esimker-com-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esimker-com/openapi/esimker-com-support-api-openapi.yml
- filename: esimker-com-telegram-api-openapi.yml
  format: yaml
  label: esimker Telegram API
  slug: esimker-com-telegram-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esimker-com/openapi/esimker-com-telegram-api-openapi.yml
- filename: esimker-com-topups-api-openapi.yml
  format: yaml
  label: esimker Topups API
  slug: esimker-com-topups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esimker-com/openapi/esimker-com-topups-api-openapi.yml
- filename: esimker-com-wallet-api-openapi.yml
  format: yaml
  label: esimker Wallet API
  slug: esimker-com-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esimker-com/openapi/esimker-com-wallet-api-openapi.yml
auth_types: []
description: Authentication methods described on the esimker API documentation page.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: esimker Authentication
name_suffix: Authentication
oauth_flows: []
overview: esimker declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: esimker
provider_slug: esimker-com
scheme_count: 2
schemes:
- evidence: 'Reseller API (reseller): white-label partners on X-API-Key, retail minus a discount; keys are issued by support.'
  header: X-API-Key
  how_to_obtain: Keys are issued by support.
  location: header
  name: X-API-Key
  type: apiKey
- evidence: 'The wallet and the catalogue are also MCP tools at POST https://esimker.com/api/mcp (Streamable HTTP; the wallet code goes in Authorization: Bearer).'
  header: Authorization
  how_to_obtain: The wallet secret code is returned when a wallet is created via POST /api/wallet.
  location: header
  name: Authorization
  type: http-bearer
slug: esimker-com-authentication
source_filename: esimker-com-authentication.yml
source_heading: Authentication Profile
source_url: https://esimker.com/api/docs
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://esimker.com/api/docs\nsources:\n- https://esimker.com/api/docs\ndescription: Authentication methods described on the esimker API documentation page.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Reseller API (reseller): white-label partners on X-API-Key, retail minus a discount; keys are issued by support.'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Keys are issued by support.\n- type: http-bearer\n  name: Authorization\n  evidence: 'The wallet and the catalogue are also MCP tools at POST https://esimker.com/api/mcp (Streamable HTTP; the wallet code goes in Authorization:\n    Bearer).'\n  location: header\n  header: Authorization\n  how_to_obtain: The wallet secret code is returned when a wallet is created via POST /api/wallet.\ndocs: https://esimker.com/api/docs\n"
source_yaml_url: https://artifacts.apis.io/esimker-com/authentication/esimker-com-authentication.yml
summary_line: 2 schemes
tags:
- Travel
- Mobile
- eSIM
- Prepaid
- International
---
