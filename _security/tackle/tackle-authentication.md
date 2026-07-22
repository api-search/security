---
api_key_in:
- header
api_specs:
- filename: tackle-api-openapi.json
  format: json
  label: Tackle API
  slug: tackle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/openapi/tackle-api-openapi.json
- filename: tackle-cosell-openapi.json
  format: json
  label: Tackle Co-Sell for AWS Partner Central
  slug: tackle-co-sell-for-aws-partner-central
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/openapi/tackle-cosell-openapi.json
- filename: tackle-marketplace-openapi.json
  format: json
  label: Tackle Offers (AWS Marketplace)
  slug: tackle-offers-aws-marketplace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/openapi/tackle-marketplace-openapi.json
- filename: tackle-offers-openapi.json
  format: json
  label: Tackle Offers (Microsoft Marketplace)
  slug: tackle-offers-microsoft-marketplace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/openapi/tackle-offers-openapi.json
- filename: tackle-contracts-openapi.json
  format: json
  label: Tackle Public Contracts API
  slug: tackle-public-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/openapi/tackle-contracts-openapi.json
- filename: tackle-prospect-openapi.json
  format: json
  label: Tackle Prospect API
  slug: tackle-prospect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/openapi/tackle-prospect-openapi.json
- filename: tackle-scim-openapi.json
  format: json
  label: Tackle SCIM API
  slug: tackle-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/openapi/tackle-scim-openapi.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Tackle Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Tackle secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Tackle
provider_slug: tackle
scheme_count: 5
schemes:
- bearerFormat: JWT
  description: The Tackle API requires a JWT for authentication. You can get this by [getting your API credentials](https://developers.tackle.io/docs/how-to-get-an-m2m-client-id-and-secret) from the Tackle Platform then [retrieving your Access Token](https://developers.tackle.io/docs/getting-an-access-token) using our Authentication endpoint.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/tackle-api-openapi.json
  - openapi/tackle-contracts-openapi.json
  - openapi/tackle-cosell-openapi.json
  - openapi/tackle-marketplace-openapi.json
  - openapi/tackle-offers-openapi.json
  - openapi/tackle-prospect-openapi.json
  type: http
- description: Use `basic` for [basic HTTP authentication](https://en.wikipedia.org/wiki/Basic_access_authentication); this is only used for `callbacks`
  name: BasicAuthCallback
  scheme: basic
  sources:
  - openapi/tackle-api-openapi.json
  type: http
- description: Use `header_api_key` to specify a custom HTTP request header for authentication. Requests from Tackle will use the specified HTTP header for outbound requests to your Webhook URL; this is only used for `callbacks`'
  in: header
  name: HeaderApiKeyAuthCallback
  parameter: subscription-key
  sources:
  - openapi/tackle-api-openapi.json
  type: apiKey
- description: This auth-type is for `oauth2` client credentials flow. We will use the client_id and client_secret to call the token_url to get an access token; this is only used for `callbacks`'
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /oauth/token
  name: Oauth2AuthCallback
  sources:
  - openapi/tackle-api-openapi.json
  type: oauth2
- description: 'API key authentication.

    Include the API key in the Authorization header.'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/tackle-scim-openapi.json
  type: apiKey
slug: tackle-authentication
source_filename: tackle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/tackle-api-openapi.json, openapi/tackle-contracts-openapi.json, openapi/tackle-cosell-openapi.json,\n  openapi/tackle-marketplace-openapi.json, openapi/tackle-offers-openapi.json, openapi/tackle-prospect-openapi.json,\n  openapi/tackle-scim-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: The Tackle API requires a JWT for authentication. You can get this by [getting\n    your API credentials](https://developers.tackle.io/docs/how-to-get-an-m2m-client-id-and-secret)\n    from the Tackle Platform then [retrieving your Access Token](https://developers.tackle.io/docs/getting-an-access-token)\n    using our Authentication endpoint.\n  sources:\n  - openapi/tackle-api-openapi.json\n  - openapi/tackle-contracts-openapi.json\n  - openapi/tackle-cosell-openapi.json\n\
  \  - openapi/tackle-marketplace-openapi.json\n  - openapi/tackle-offers-openapi.json\n  - openapi/tackle-prospect-openapi.json\n- name: BasicAuthCallback\n  type: http\n  scheme: basic\n  description: Use `basic` for [basic HTTP authentication](https://en.wikipedia.org/wiki/Basic_access_authentication);\n    this is only used for `callbacks`\n  sources:\n  - openapi/tackle-api-openapi.json\n- name: HeaderApiKeyAuthCallback\n  type: apiKey\n  in: header\n  parameter: subscription-key\n  description: Use `header_api_key` to specify a custom HTTP request header for authentication.\n    Requests from Tackle will use the specified HTTP header for outbound requests to your Webhook\n    URL; this is only used for `callbacks`'\n  sources:\n  - openapi/tackle-api-openapi.json\n- name: Oauth2AuthCallback\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n    scopes: 0\n  description: This auth-type is for `oauth2` client credentials flow. We will use the client_id\n\
  \    and client_secret to call the token_url to get an access token; this is only used for `callbacks`'\n  sources:\n  - openapi/tackle-api-openapi.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    API key authentication.\n    Include the API key in the Authorization header.\n  sources:\n  - openapi/tackle-scim-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/authentication/tackle-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Company
- Cloud Marketplace
- Cloud GTM
- Go-To-Market
- Private Offers
- Co-Sell
- Metering
- SCIM
- AWS Marketplace
- Azure Marketplace
---
