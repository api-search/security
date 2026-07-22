---
api_key_in:
- header
api_specs:
- filename: tackleio-platform-openapi.json
  format: json
  label: Tackle Platform API
  slug: tackle-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-platform-openapi.json
- filename: tackleio-prospect-openapi.json
  format: json
  label: Tackle Prospect API
  slug: tackle-prospect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-prospect-openapi.json
- filename: tackleio-cosell-aws-openapi.json
  format: json
  label: Tackle Co-Sell for AWS Partner Central
  slug: tackle-co-sell-for-aws-partner-central
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-cosell-aws-openapi.json
- filename: tackleio-cosell-gcp-openapi.json
  format: json
  label: Tackle Co-Sell for Google Cloud
  slug: tackle-co-sell-for-google-cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-cosell-gcp-openapi.json
- filename: tackleio-cosell-msft-openapi.json
  format: json
  label: Tackle Co-Sell for Microsoft Partner Center
  slug: tackle-co-sell-for-microsoft-partner-center
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-cosell-msft-openapi.json
- filename: tackleio-offers-aws-openapi.json
  format: json
  label: Tackle Offers for AWS Marketplace
  slug: tackle-offers-for-aws-marketplace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-offers-aws-openapi.json
- filename: tackleio-offers-msft-openapi.json
  format: json
  label: Tackle Offers for Microsoft
  slug: tackle-offers-for-microsoft
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-offers-msft-openapi.json
- filename: tackleio-contracts-openapi.json
  format: json
  label: Tackle Public Contracts API
  slug: tackle-public-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-contracts-openapi.json
- filename: tackleio-scim-openapi.json
  format: json
  label: Tackle SCIM API
  slug: tackle-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-scim-openapi.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Tackleio Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Tackle.io secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Tackle.io
provider_slug: tackleio
scheme_count: 5
schemes:
- bearerFormat: JWT
  description: Tackle-issued JWT (interactive user or MTM token).
  name: tackleJwt
  scheme: bearer
  sources:
  - openapi/tackleio-contracts-openapi.json
  - openapi/tackleio-cosell-aws-openapi.json
  - openapi/tackleio-cosell-gcp-openapi.json
  - openapi/tackleio-cosell-msft-openapi.json
  - openapi/tackleio-offers-aws-openapi.json
  - openapi/tackleio-offers-msft-openapi.json
  - openapi/tackleio-platform-openapi.json
  - openapi/tackleio-prospect-openapi.json
  type: http
- description: Use `basic` for [basic HTTP authentication](https://en.wikipedia.org/wiki/Basic_access_authentication); this is only used for `callbacks`
  name: BasicAuthCallback
  scheme: basic
  sources:
  - openapi/tackleio-platform-openapi.json
  type: http
- description: Use `header_api_key` to specify a custom HTTP request header for authentication. Requests from Tackle will use the specified HTTP header for outbound requests to your Webhook URL; this is only used for `callbacks`'
  in: header
  name: HeaderApiKeyAuthCallback
  parameter: subscription-key
  sources:
  - openapi/tackleio-platform-openapi.json
  type: apiKey
- description: This auth-type is for `oauth2` client credentials flow. We will use the client_id and client_secret to call the token_url to get an access token; this is only used for `callbacks`'
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /oauth/token
  name: Oauth2AuthCallback
  sources:
  - openapi/tackleio-platform-openapi.json
  type: oauth2
- description: 'API key authentication.

    Include the API key in the Authorization header.'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/tackleio-scim-openapi.json
  type: apiKey
slug: tackleio-authentication
source_filename: tackleio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/tackleio-contracts-openapi.json, openapi/tackleio-cosell-aws-openapi.json, openapi/tackleio-cosell-gcp-openapi.json,\n  openapi/tackleio-cosell-msft-openapi.json, openapi/tackleio-offers-aws-openapi.json, openapi/tackleio-offers-msft-openapi.json,\n  openapi/tackleio-platform-openapi.json, openapi/tackleio-prospect-openapi.json, openapi/tackleio-scim-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: tackleJwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Tackle-issued JWT (interactive user or MTM token).\n  sources:\n  - openapi/tackleio-contracts-openapi.json\n  - openapi/tackleio-cosell-aws-openapi.json\n  - openapi/tackleio-cosell-gcp-openapi.json\n  - openapi/tackleio-cosell-msft-openapi.json\n  - openapi/tackleio-offers-aws-openapi.json\n  - openapi/tackleio-offers-msft-openapi.json\n  -\
  \ openapi/tackleio-platform-openapi.json\n  - openapi/tackleio-prospect-openapi.json\n- name: BasicAuthCallback\n  type: http\n  scheme: basic\n  description: Use `basic` for [basic HTTP authentication](https://en.wikipedia.org/wiki/Basic_access_authentication);\n    this is only used for `callbacks`\n  sources:\n  - openapi/tackleio-platform-openapi.json\n- name: HeaderApiKeyAuthCallback\n  type: apiKey\n  in: header\n  parameter: subscription-key\n  description: Use `header_api_key` to specify a custom HTTP request header for authentication. Requests\n    from Tackle will use the specified HTTP header for outbound requests to your Webhook URL; this is\n    only used for `callbacks`'\n  sources:\n  - openapi/tackleio-platform-openapi.json\n- name: Oauth2AuthCallback\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n    scopes: 0\n  description: This auth-type is for `oauth2` client credentials flow. We will use the client_id and client_secret\n    to\
  \ call the token_url to get an access token; this is only used for `callbacks`'\n  sources:\n  - openapi/tackleio-platform-openapi.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key authentication.\n\n    Include the API key in the Authorization header.'\n  sources:\n  - openapi/tackleio-scim-openapi.json\ndocs: https://developers.tackle.io/docs/getting-an-access-token\ntoken_endpoint: POST https://api.tackle.io/v1/authenticate\ngrant: client_credentials (machine-to-machine)\nidp: 'Auth0 tenant https://auth.tackle.io (OIDC: https://auth.tackle.io/.well-known/openid-configuration)'\ntoken_ttl_seconds: 5400\nnotes: 'Primary API auth is an OAuth2 client-credentials JWT (Authorization: Bearer). The SCIM service\n  uses a static API key. Basic/header-api-key/oauth2 callback schemes secure outbound webhook delivery\n  only.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/authentication/tackleio-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Company
- Cloud
- Cloud Marketplace
- Co-Sell
- AWS Marketplace
- Azure Marketplace
- Google Cloud Marketplace
- Private Offers
- Metering
- SCIM
- Webhooks
- B2B SaaS
---
