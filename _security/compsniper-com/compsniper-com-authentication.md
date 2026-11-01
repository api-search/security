---
anonymous_access: false
api_key_in: []
api_specs:
- filename: compsniper-com-account-api-openapi.yml
  format: yaml
  label: compsniper-com Account API
  slug: compsniper-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-account-api-openapi.yml
- filename: compsniper-com-best-offer-prices-api-openapi.yml
  format: yaml
  label: compsniper-com Best Offer Prices API
  slug: compsniper-com-best-offer-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-best-offer-prices-api-openapi.yml
- filename: compsniper-com-bulk-search-api-openapi.yml
  format: yaml
  label: compsniper-com Bulk Search API
  slug: compsniper-com-bulk-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-bulk-search-api-openapi.yml
- filename: compsniper-com-cards-api-openapi.yml
  format: yaml
  label: compsniper-com Cards API
  slug: compsniper-com-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-cards-api-openapi.yml
- filename: compsniper-com-depop-api-openapi.yml
  format: yaml
  label: compsniper-com Depop API
  slug: compsniper-com-depop-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-depop-api-openapi.yml
- filename: compsniper-com-grailed-api-openapi.yml
  format: yaml
  label: compsniper-com Grailed API
  slug: compsniper-com-grailed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-grailed-api-openapi.yml
- filename: compsniper-com-mercari-api-openapi.yml
  format: yaml
  label: compsniper-com Mercari API
  slug: compsniper-com-mercari-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-mercari-api-openapi.yml
- filename: compsniper-com-poshmark-api-openapi.yml
  format: yaml
  label: compsniper-com Poshmark API
  slug: compsniper-com-poshmark-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-poshmark-api-openapi.yml
- filename: compsniper-com-psa-api-openapi.yml
  format: yaml
  label: compsniper-com PSA API
  slug: compsniper-com-psa-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-psa-api-openapi.yml
- filename: compsniper-com-scrape-api-openapi.yml
  format: yaml
  label: compsniper-com Scrape API
  slug: compsniper-com-scrape-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-scrape-api-openapi.yml
- filename: compsniper-com-shipping-rates-api-openapi.yml
  format: yaml
  label: compsniper-com Shipping Rates API
  slug: compsniper-com-shipping-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-shipping-rates-api-openapi.yml
- filename: compsniper-com-sold-history-api-openapi.yml
  format: yaml
  label: compsniper-com Sold history API
  slug: compsniper-com-sold-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-sold-history-api-openapi.yml
- filename: compsniper-com-summary-api-openapi.yml
  format: yaml
  label: compsniper-com Summary API
  slug: compsniper-com-summary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-summary-api-openapi.yml
- filename: compsniper-com-tcgplayer-api-openapi.yml
  format: yaml
  label: compsniper-com TC Gplayer API
  slug: compsniper-com-tcgplayer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-tcgplayer-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Compsniper Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: compsniper-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: compsniper-com
provider_slug: compsniper-com
scheme_count: 2
schemes:
- description: 'Bearer token for API key authentication (e.g., "Authorization: Bearer cs_live_...")

    '
  in: header
  name: Authorization
  type: apiKey
- flows:
    authorizationCode:
      authorizationUrl: https://compsniper.com/oauth/authorize
      scopes:
        account:read: Read plan and remaining quota
        comps:read: Search and compare sold listings
        jobs:write: Start and cancel Max Mode jobs
        offline_access: Refresh the approved connection
      tokenUrl: https://compsniper.com/oauth/token
  type: oauth2
slug: compsniper-com-authentication
source_filename: compsniper-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://compsniper.com/docs/authentication.md\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: |\n      Bearer token for API key authentication (e.g., \"Authorization: Bearer cs_live_...\")\n  - type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://compsniper.com/oauth/authorize\n        tokenUrl: https://compsniper.com/oauth/token\n        scopes:\n          comps:read: Search and compare sold listings\n          account:read: Read plan and remaining quota\n          jobs:write: Start and cancel Max Mode jobs\n          offline_access: Refresh the approved connection"
source_yaml_url: https://artifacts.apis.io/compsniper-com/authentication/compsniper-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- API
- Marketplace
- E-commerce
- Data
- Collectibles
---
