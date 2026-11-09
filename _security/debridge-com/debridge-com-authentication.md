---
anonymous_access: false
api_key_in: []
api_specs:
- filename: debridge-com-appcontrollerv10-api-openapi.yml
  format: yaml
  label: deBridge App Controller V10 API
  slug: debridge-com-appcontrollerv10-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-appcontrollerv10-api-openapi.yml
- filename: debridge-com-dln-api-openapi.yml
  format: yaml
  label: deBridge DLN API
  slug: debridge-com-dln-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-dln-api-openapi.yml
- filename: debridge-com-orders-api-openapi.yml
  format: yaml
  label: deBridge Orders API
  slug: debridge-com-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-orders-api-openapi.yml
- filename: debridge-com-samechainswap-api-openapi.yml
  format: yaml
  label: deBridge Same Chain Swap API
  slug: debridge-com-samechainswap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-samechainswap-api-openapi.yml
- filename: debridge-com-satistics-api-openapi.yml
  format: yaml
  label: deBridge Satistics API
  slug: debridge-com-satistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-satistics-api-openapi.yml
- filename: debridge-com-single-chain-swap-api-openapi.yml
  format: yaml
  label: deBridge single chain swap API
  slug: debridge-com-single-chain-swap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-single-chain-swap-api-openapi.yml
- filename: debridge-com-tokenmetadata-api-openapi.yml
  format: yaml
  label: deBridge Token Metadata API
  slug: debridge-com-tokenmetadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-tokenmetadata-api-openapi.yml
- filename: debridge-com-transaction-api-openapi.yml
  format: yaml
  label: deBridge Transaction API
  slug: debridge-com-transaction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-transaction-api-openapi.yml
- filename: debridge-com-users-api-openapi.yml
  format: yaml
  label: deBridge Users API
  slug: debridge-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-users-api-openapi.yml
- filename: debridge-com-utils-api-openapi.yml
  format: yaml
  label: deBridge Utils API
  slug: debridge-com-utils-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-utils-api-openapi.yml
- filename: debridge-com-order-events-api-openapi.yml
  format: yaml
  label: deBridge Order Events API
  slug: debridge-com-order-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-order-events-api-openapi.yml
- filename: debridge-com-referral-program-api-openapi.yml
  format: yaml
  label: deBridge Referral Program API
  slug: debridge-com-referral-program-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-referral-program-api-openapi.yml
- filename: debridge-com-terms-and-conditions-api-openapi.yml
  format: yaml
  label: deBridge Terms And Conditions API
  slug: debridge-com-terms-and-conditions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-terms-and-conditions-api-openapi.yml
auth_types: []
description: Authentication requirements and rate limits for the DLN API.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Debridge Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: deBridge declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: deBridge
provider_slug: debridge-com
scheme_count: 1
schemes:
- evidence: The DLN API is open to everyone with a limited RPS and doesn't require authentication. To make sure we keep delivering a high-quality service, we've introduced a requirement for commercial integrations to authenticate requests with dedicated API keys.
  how_to_obtain: Fill in the Authentication Request form at https://forms.gle/doWLQpr8oemphoaf9 to receive a dedicated API key.
  name: API key
  type: apiKey
slug: debridge-com-authentication
source_filename: debridge-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.debridge.com/dln-details/integration-guidelines/order-creation/authentication.md
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.debridge.com/dln-details/integration-guidelines/order-creation/authentication.md\nsources:\n- https://docs.debridge.com/dln-details/integration-guidelines/order-creation/authentication.md\n- https://docs.debridge.com/home/resources/supported-tokens.md\n- https://docs.debridge.com/api-reference/tokenmetadata/get-list-of-tokens-transferred-with-dln-sorted-by-popularity.md\ndescription: Authentication requirements and rate limits for the DLN API.\nschemes:\n- type: apiKey\n  name: API key\n  evidence: The DLN API is open to everyone with a limited RPS and doesn't require authentication. To make sure we keep delivering a high-quality\n    service, we've introduced a requirement for commercial integrations to authenticate requests with dedicated API keys.\n  how_to_obtain: Fill in the Authentication Request form at https://forms.gle/doWLQpr8oemphoaf9 to receive a dedicated\
  \ API key.\nnote: No other authentication schemes are documented.\ndocs: https://docs.debridge.com/dln-details/integration-guidelines/order-creation/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/debridge-com/authentication/debridge-com-authentication.yml
summary_line: 1 scheme
tags:
- Cross-Chain Bridge
- DeFi Infrastructure
- Crypto Swaps
- Analytics
---
