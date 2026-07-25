---
api_key_in:
- header
api_specs:
- filename: swagger
  format: yaml
  label: Reverb REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://reverb.com/swagger
- filename: reverb-accounts-api-openapi.yml
  format: yaml
  label: Reverb Accounts API
  slug: reverb-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/openapi/reverb-accounts-api-openapi.yml
- filename: reverb-articles-api-openapi.yml
  format: yaml
  label: Reverb Articles API
  slug: reverb-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/openapi/reverb-articles-api-openapi.yml
- filename: reverb-auth-api-openapi.yml
  format: yaml
  label: Reverb Auth API
  slug: reverb-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/openapi/reverb-auth-api-openapi.yml
- filename: reverb-autocomplete-api-openapi.yml
  format: yaml
  label: Reverb Autocomplete API
  slug: reverb-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/openapi/reverb-autocomplete-api-openapi.yml
- filename: reverb-autosuggest-api-openapi.yml
  format: yaml
  label: Reverb Autosuggest API
  slug: reverb-autosuggest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/openapi/reverb-autosuggest-api-openapi.yml
- filename: reverb-braintree-api-openapi.yml
  format: yaml
  label: Reverb Braintree API
  slug: reverb-braintree-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/openapi/reverb-braintree-api-openapi.yml
- filename: reverb-cart-api-openapi.yml
  format: yaml
  label: Reverb Cart API
  slug: reverb-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/openapi/reverb-cart-api-openapi.yml
- filename: reverb-categories-api-openapi.yml
  format: yaml
  label: Reverb Categories API
  slug: reverb-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/openapi/reverb-categories-api-openapi.yml
- filename: reverb-collections-api-openapi.yml
  format: yaml
  label: Reverb Collections API
  slug: reverb-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/openapi/reverb-collections-api-openapi.yml
- filename: reverb-countries-api-openapi.yml
  format: yaml
  label: Reverb Countries API
  slug: reverb-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/openapi/reverb-countries-api-openapi.yml
- filename: reverb-currencies-api-openapi.yml
  format: yaml
  label: Reverb Currencies API
  slug: reverb-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/openapi/reverb-currencies-api-openapi.yml
- filename: reverb-listings-api-openapi.yml
  format: yaml
  label: Reverb Listings API
  slug: reverb-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/openapi/reverb-listings-api-openapi.yml
- filename: reverb-my-api-openapi.yml
  format: yaml
  label: Reverb My API
  slug: reverb-my-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/openapi/reverb-my-api-openapi.yml
- filename: reverb-payment-methods-api-openapi.yml
  format: yaml
  label: Reverb Payment Methods API
  slug: reverb-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/openapi/reverb-payment-methods-api-openapi.yml
- filename: reverb-priceguide-api-openapi.yml
  format: yaml
  label: Reverb Priceguide API
  slug: reverb-priceguide-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/openapi/reverb-priceguide-api-openapi.yml
- filename: reverb-push-notifications-api-openapi.yml
  format: yaml
  label: Reverb Push Notifications API
  slug: reverb-push-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/openapi/reverb-push-notifications-api-openapi.yml
- filename: reverb-reverb-api-api-openapi.yml
  format: yaml
  label: Reverb Reverb API API
  slug: reverb-reverb-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/openapi/reverb-reverb-api-api-openapi.yml
- filename: reverb-shipping-api-openapi.yml
  format: yaml
  label: Reverb Shipping API
  slug: reverb-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/openapi/reverb-shipping-api-openapi.yml
- filename: reverb-shop-api-openapi.yml
  format: yaml
  label: Reverb Shop API
  slug: reverb-shop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/openapi/reverb-shop-api-openapi.yml
- filename: reverb-wants-api-openapi.yml
  format: yaml
  label: Reverb Wants API
  slug: reverb-wants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/openapi/reverb-wants-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Reverb Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reverb secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reverb
provider_slug: reverb
scheme_count: 1
schemes:
- description: 'Token returned by POST /api/auth/tokens, supplied on subsequent calls in

    the `X-Auth-Token` request header.'
  in: header
  name: XAuthToken
  parameter: X-Auth-Token
  sources:
  - openapi/reverb-openapi.yml
  type: apiKey
slug: reverb-authentication
source_filename: reverb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reverb-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: XAuthToken\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  description: |-\n    Token returned by POST /api/auth/tokens, supplied on subsequent calls in\n    the `X-Auth-Token` request header.\n  sources:\n  - openapi/reverb-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/authentication/reverb-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Marketplace
- Music
- Instruments
- Ecommerce
---
