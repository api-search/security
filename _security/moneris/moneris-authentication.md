---
api_key_in:
- header
api_specs:
- filename: moneris-3d-secure-api-openapi.yml
  format: yaml
  label: Moneris 3D Secure API
  slug: moneris-3d-secure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-3d-secure-api-openapi.yml
- filename: moneris-customers-api-openapi.yml
  format: yaml
  label: Moneris Customers API
  slug: moneris-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-customers-api-openapi.yml
- filename: moneris-disputes-api-openapi.yml
  format: yaml
  label: Moneris Disputes API
  slug: moneris-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-disputes-api-openapi.yml
- filename: moneris-installments-api-openapi.yml
  format: yaml
  label: Moneris Installments API
  slug: moneris-installments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-installments-api-openapi.yml
- filename: moneris-kount-api-openapi.yml
  format: yaml
  label: Moneris Kount API
  slug: moneris-kount-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-kount-api-openapi.yml
- filename: moneris-merchant-onboarding-api-openapi.yml
  format: yaml
  label: Moneris Merchant Onboarding API
  slug: moneris-merchant-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-merchant-onboarding-api-openapi.yml
- filename: moneris-multi-currency-pricing-rate-lookup-api-openapi.yml
  format: yaml
  label: Moneris Multi-Currency Pricing Rate Lookup API
  slug: moneris-multi-currency-pricing-rate-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-multi-currency-pricing-rate-lookup-api-openapi.yml
- filename: moneris-payment-methods-api-openapi.yml
  format: yaml
  label: Moneris Payment Methods API
  slug: moneris-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-payment-methods-api-openapi.yml
- filename: moneris-payments-api-openapi.yml
  format: yaml
  label: Moneris Payments API
  slug: moneris-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-payments-api-openapi.yml
- filename: moneris-products-api-openapi.yml
  format: yaml
  label: Moneris Products API
  slug: moneris-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-products-api-openapi.yml
- filename: moneris-refunds-api-openapi.yml
  format: yaml
  label: Moneris Refunds API
  slug: moneris-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-refunds-api-openapi.yml
- filename: moneris-subscriptions-api-openapi.yml
  format: yaml
  label: Moneris Subscriptions API
  slug: moneris-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-subscriptions-api-openapi.yml
- filename: moneris-surcharge-lookup-api-openapi.yml
  format: yaml
  label: Moneris Surcharge Lookup API
  slug: moneris-surcharge-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-surcharge-lookup-api-openapi.yml
- filename: moneris-terminal-service-orders-api-openapi.yml
  format: yaml
  label: Moneris Terminal & Service Orders API
  slug: moneris-terminal-service-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-terminal-service-orders-api-openapi.yml
- filename: moneris-validations-api-openapi.yml
  format: yaml
  label: Moneris Validations API
  slug: moneris-validations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-validations-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Moneris Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Moneris secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Moneris
provider_slug: moneris
scheme_count: 2
schemes:
- description: 'An API key is a token that a client provides when making API calls.


    API keys are supposed to be a secret that only the client and server know about.'
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/moneris-unified-api-openapi.json
  type: apiKey
- description: 'OAuth 2.0 is an authorization protocol that gives an API client limited access to user data on a web server.


    OAuth relies on authentication scenarios, that allows the resource owner (user) to share the protected content from the server, hosting the resource, without sharing their credentials. For that purpose, an OAuth 2.0 server issues access tokens that the client applications can use to access'
  flows:
  - flow: clientCredentials
    scopes: 14
    tokenUrl: /oauth2/token
  name: OAuth2
  sources:
  - openapi/moneris-unified-api-openapi.json
  type: oauth2
slug: moneris-authentication
source_filename: moneris-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: openapi/moneris-unified-api-openapi.json\ndocs: https://developer.moneris.com/moneris-api/docs/authentication-api-keys\nnotes: >-\n  Moneris recommends OAuth 2.0 client-credentials (POST /oauth2/token,\n  grant_type=client_credentials, scope-limited) over the X-Api-Key header. Both\n  Client Credentials apps and API Key \"subscriptions\" are self-provisioned from\n  the Developer Portal Access & Credentials page (max 2 of each per account);\n  sandbox and production credentials are separate.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: |-\n    An API key is a token that a client provides when making API calls.\n\n    API keys are supposed to be a secret that only the client and server know about.\n  sources:\n  - openapi/moneris-unified-api-openapi.json\n- name:\
  \ OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/token\n    scopes: 14\n  description: |-\n    OAuth 2.0 is an authorization protocol that gives an API client limited access to user data on a web server.\n\n    OAuth relies on authentication scenarios, that allows the resource owner (user) to share the protected content from the server, hosting the resource, without sharing their credentials. For that purpose, an OAuth 2.0 server issues access tokens that the client applications can use to access\n  sources:\n  - openapi/moneris-unified-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/authentication/moneris-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Financial-Services
- Payments
- Payment Processing
- Card Payments
- Merchant Services
- Acquiring
- Canada
- Fintech
- Infrastructure
---
