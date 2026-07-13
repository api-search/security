---
api_key_in:
- query
api_specs:
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Storefront Products API
  slug: fourthwall-storefront-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Storefront Collections API
  slug: fourthwall-storefront-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Storefront Cart & Checkout API
  slug: fourthwall-storefront-cart-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Orders API
  slug: fourthwall-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Products API
  slug: fourthwall-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Gifting & Giveaways API
  slug: fourthwall-gifting-giveaways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Promotions API
  slug: fourthwall-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Memberships API
  slug: fourthwall-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Webhooks API
  slug: fourthwall-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Fourthwall Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Fourthwall secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Fourthwall
provider_slug: fourthwall
scheme_count: 3
schemes:
- description: Public storefront token obtained from Settings > For Developers, passed as the storefront_token query parameter on Storefront API requests.
  in: query
  name: storefrontToken
  parameter: storefront_token
  sources:
  - openapi/fourthwall-openapi.yml
  type: apiKey
- description: Shop API key used with HTTP Basic Authentication against the Platform (Open) API.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/fourthwall-openapi.yml
  type: http
- description: OAuth 2.0 for multi-shop platform apps.
  flows:
  - authorizationUrl: https://auth.fourthwall.com/auth/realms/Fourthwall/protocol/openid-connect/auth
    flow: authorizationCode
    scopes: 14
    tokenUrl: https://api.fourthwall.com/open-api/v1.0/platform/token
  name: oauth
  sources:
  - openapi/fourthwall-openapi.yml
  type: oauth2
slug: fourthwall-authentication
source_filename: fourthwall-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fourthwall-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: storefrontToken\n  type: apiKey\n  in: query\n  parameter: storefront_token\n  description: Public storefront token obtained from Settings > For Developers, passed as the\n    storefront_token query parameter on Storefront API requests.\n  sources:\n  - openapi/fourthwall-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Shop API key used with HTTP Basic Authentication against the Platform (Open)\n    API.\n  sources:\n  - openapi/fourthwall-openapi.yml\n- name: oauth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.fourthwall.com/auth/realms/Fourthwall/protocol/openid-connect/auth\n    tokenUrl: https://api.fourthwall.com/open-api/v1.0/platform/token\n    scopes: 14\n  description: OAuth\
  \ 2.0 for multi-shop platform apps.\n  sources:\n  - openapi/fourthwall-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/authentication/fourthwall-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Creator Commerce
- Ecommerce
- Merch
- Storefront
- Memberships
- Donations
- Print on Demand
---
