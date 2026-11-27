---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication uses a Bearer token sent in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: MarketBasketAnalysis Authentication
name_suffix: Authentication
oauth_flows: []
overview: MarketBasketAnalysis declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MarketBasketAnalysis
provider_slug: marketbasketanalysis-com
scheme_count: 1
schemes:
- evidence: 'Auth scheme Bearer token on Shopify, BigCommerce, and WooCommerce: send Authorization: Bearer mba_live_... on every request.'
  header: Authorization
  how_to_obtain: Mint an API key in the MBA admin (Settings > API keys) and copy the plaintext mba_live_... token.
  location: header
  name: Bearer
  type: http-bearer
slug: marketbasketanalysis-com-authentication
source_filename: marketbasketanalysis-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.marketbasketanalysis.com/docs/api
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.marketbasketanalysis.com/docs/api\nsources:\n- https://www.marketbasketanalysis.com/docs/api\n- https://www.marketbasketanalysis.com/docs/mcp\ndescription: Authentication uses a Bearer token sent in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Auth scheme Bearer token on Shopify, BigCommerce, and WooCommerce: send Authorization: Bearer mba_live_... on every request.'\n  location: header\n  header: Authorization\n  how_to_obtain: Mint an API key in the MBA admin (Settings > API keys) and copy the plaintext mba_live_... token.\nnote: No OAuth2, API key query, or other authentication methods are documented.\ndocs: https://www.marketbasketanalysis.com/docs/api\n"
source_yaml_url: https://artifacts.apis.io/marketbasketanalysis-com/authentication/marketbasketanalysis-com-authentication.yml
summary_line: 1 scheme
tags:
- Upsell
- Shopify
- BigCommerce
- WooCommerce
- Magento
---
