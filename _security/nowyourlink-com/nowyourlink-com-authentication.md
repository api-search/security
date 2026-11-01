---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nowyourlink-com-affiliate-api-openapi.yml
  format: yaml
  label: nowyourlink-com Affiliate API
  slug: nowyourlink-com-affiliate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowyourlink-com/openapi/nowyourlink-com-affiliate-api-openapi.yml
- filename: nowyourlink-com-agent-api-openapi.yml
  format: yaml
  label: nowyourlink-com Agent API
  slug: nowyourlink-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowyourlink-com/openapi/nowyourlink-com-agent-api-openapi.yml
- filename: nowyourlink-com-ask-api-openapi.yml
  format: yaml
  label: nowyourlink-com Ask API
  slug: nowyourlink-com-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowyourlink-com/openapi/nowyourlink-com-ask-api-openapi.yml
- filename: nowyourlink-com-checkout-sessions-api-openapi.yml
  format: yaml
  label: nowyourlink-com Checkout Sessions API
  slug: nowyourlink-com-checkout-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowyourlink-com/openapi/nowyourlink-com-checkout-sessions-api-openapi.yml
- filename: nowyourlink-com-sandbox-api-openapi.yml
  format: yaml
  label: nowyourlink-com Sandbox API
  slug: nowyourlink-com-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowyourlink-com/openapi/nowyourlink-com-sandbox-api-openapi.yml
- filename: nowyourlink-com-spotlight-api-openapi.yml
  format: yaml
  label: nowyourlink-com Spotlight API
  slug: nowyourlink-com-spotlight-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowyourlink-com/openapi/nowyourlink-com-spotlight-api-openapi.yml
- filename: nowyourlink-com-spotlights-api-openapi.yml
  format: yaml
  label: nowyourlink-com Spotlights API
  slug: nowyourlink-com-spotlights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowyourlink-com/openapi/nowyourlink-com-spotlights-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Nowyourlink Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: nowyourlink-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: nowyourlink-com
provider_slug: nowyourlink-com
scheme_count: 1
schemes:
- authorizationUrl: https://api.nowyourlink.com/oauth/authorize
  flow: authorizationCode
  pkce: true
  refreshUrl: https://api.nowyourlink.com/oauth/token
  scopes:
    account:read: Read account information
    affiliate:read: Read affiliate data
    affiliate:write: Modify affiliate data
    bids:read: Read bids
    bids:write: Create or modify bids
    creatives:read: Read creative assets
    creatives:write: Create or modify creatives
    invoices:read: Read invoices
  tokenUrl: https://api.nowyourlink.com/oauth/token
  type: oauth2
slug: nowyourlink-com-authentication
source_filename: nowyourlink-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: \"https://nowyourlink.com/auth.md\"\nschemes:\n  - type: oauth2\n    flow: authorizationCode\n    pkce: true\n    authorizationUrl: https://api.nowyourlink.com/oauth/authorize\n    tokenUrl: https://api.nowyourlink.com/oauth/token\n    refreshUrl: https://api.nowyourlink.com/oauth/token\n    scopes:\n      account:read: \"Read account information\"\n      bids:read: \"Read bids\"\n      bids:write: \"Create or modify bids\"\n      creatives:read: \"Read creative assets\"\n      creatives:write: \"Create or modify creatives\"\n      invoices:read: \"Read invoices\"\n      affiliate:read: \"Read affiliate data\"\n      affiliate:write: \"Modify affiliate data\"\n"
source_yaml_url: https://artifacts.apis.io/nowyourlink-com/authentication/nowyourlink-com-authentication.yml
summary_line: 1 scheme
tags:
- Advertising
- Marketplace
- Auction
- API
- Technology
---
