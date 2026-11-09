---
anonymous_access: false
api_key_in: []
api_specs:
- filename: buyukesim-com-bundle-crypto-quote-php-api-openapi.yml
  format: yaml
  label: BuyUKeSIM Bundle Crypto Quote.php API
  slug: buyukesim-com-bundle-crypto-quote-php-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyukesim-com/openapi/buyukesim-com-bundle-crypto-quote-php-api-openapi.yml
- filename: buyukesim-com-crypto-quote-php-api-openapi.yml
  format: yaml
  label: BuyUKeSIM Crypto Quote.php API
  slug: buyukesim-com-crypto-quote-php-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyukesim-com/openapi/buyukesim-com-crypto-quote-php-api-openapi.yml
- filename: buyukesim-com-payment-methods-php-api-openapi.yml
  format: yaml
  label: BuyUKeSIM Payment Methods.php API
  slug: buyukesim-com-payment-methods-php-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyukesim-com/openapi/buyukesim-com-payment-methods-php-api-openapi.yml
- filename: buyukesim-com-reviews-list-php-api-openapi.yml
  format: yaml
  label: BuyUKeSIM Reviews List.php API
  slug: buyukesim-com-reviews-list-php-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyukesim-com/openapi/buyukesim-com-reviews-list-php-api-openapi.yml
- filename: buyukesim-com-topup-quote-php-api-openapi.yml
  format: yaml
  label: BuyUKeSIM Topup Quote.php API
  slug: buyukesim-com-topup-quote-php-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyukesim-com/openapi/buyukesim-com-topup-quote-php-api-openapi.yml
- filename: buyukesim-com-travel-crypto-quote-php-api-openapi.yml
  format: yaml
  label: BuyUKeSIM Travel Crypto Quote.php API
  slug: buyukesim-com-travel-crypto-quote-php-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyukesim-com/openapi/buyukesim-com-travel-crypto-quote-php-api-openapi.yml
- filename: buyukesim-com-travel-packages-php-api-openapi.yml
  format: yaml
  label: BuyUKeSIM Travel Packages.php API
  slug: buyukesim-com-travel-packages-php-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyukesim-com/openapi/buyukesim-com-travel-packages-php-api-openapi.yml
- filename: buyukesim-com-vpn-crypto-quote-php-api-openapi.yml
  format: yaml
  label: BuyUKeSIM Vpn Crypto Quote.php API
  slug: buyukesim-com-vpn-crypto-quote-php-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyukesim-com/openapi/buyukesim-com-vpn-crypto-quote-php-api-openapi.yml
- filename: buyukesim-com-vpn-plans-php-api-openapi.yml
  format: yaml
  label: BuyUKeSIM Vpn Plans.php API
  slug: buyukesim-com-vpn-plans-php-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyukesim-com/openapi/buyukesim-com-vpn-plans-php-api-openapi.yml
auth_types: []
description: BuyUKeSIM uses a prepaid wallet key (api_key) for authentication on the wallet server.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Buyukesim Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: BuyUKeSIM declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: BuyUKeSIM
provider_slug: buyukesim-com
scheme_count: 2
schemes:
- evidence: 'An `Authorization: Bearer ak_live_...` header works too and takes lower precedence, but the argument is the form to prefer.'
  header: Authorization
  how_to_obtain: Call `create_wallet` on https://buyukesim.com/mcp which returns an `api_key` of the form `ak_live_...`.
  location: header
  name: Authorization
  type: apiKey
- evidence: POST https://buyukesim.com/mcp/ak_live_YOURKEY Key-in-URL form. Same endpoint, but your API key is in the path, so no header is needed.
  how_to_obtain: Call `create_wallet` on https://buyukesim.com/mcp which returns an `api_key` of the form `ak_live_...`.
  location: path
  name: ak_live_YOURKEY
  type: apiKey
slug: buyukesim-com-authentication
source_filename: buyukesim-com-authentication.yml
source_heading: Authentication Profile
source_url: https://buyukesim.com/auth.md
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://buyukesim.com/auth.md\nsources:\n- https://buyukesim.com/auth.md\n- https://buyukesim.com/en/phone-number-for-two-factor-authentication/\n- https://mcp.buyukesim.com\n- https://buyukesim.com/en/mcp-docs/\ndescription: BuyUKeSIM uses a prepaid wallet key (api_key) for authentication on the wallet server.\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: 'An `Authorization: Bearer ak_live_...` header works too and takes lower precedence, but the argument is the form to prefer.'\n  location: header\n  header: Authorization\n  how_to_obtain: Call `create_wallet` on https://buyukesim.com/mcp which returns an `api_key` of the form `ak_live_...`.\n- type: apiKey\n  name: ak_live_YOURKEY\n  evidence: POST https://buyukesim.com/mcp/ak_live_YOURKEY Key-in-URL form. Same endpoint, but your API key is in the path, so no header is needed.\n  location: path\n  how_to_obtain:\
  \ Call `create_wallet` on https://buyukesim.com/mcp which returns an `api_key` of the form `ak_live_...`.\nnote: No OAuth flows, no other authentication types are documented.\ndocs: https://buyukesim.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/buyukesim-com/authentication/buyukesim-com-authentication.yml
summary_line: 2 schemes
tags:
- eSIM
- Cryptocurrency
- Privacy
- Telecommunications
- Travel
---
