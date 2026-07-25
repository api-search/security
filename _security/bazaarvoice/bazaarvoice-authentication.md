---
api_key_in:
- header
- query
api_specs:
- filename: bazaarvoice-answers-api-openapi.yml
  format: yaml
  label: Bazaarvoice Answers API
  slug: bazaarvoice-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-answers-api-openapi.yml
- filename: bazaarvoice-clients-api-openapi.yml
  format: yaml
  label: Bazaarvoice Clients API
  slug: bazaarvoice-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-clients-api-openapi.yml
- filename: bazaarvoice-contributor-api-openapi.yml
  format: yaml
  label: Bazaarvoice Contributor API
  slug: bazaarvoice-contributor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-contributor-api-openapi.yml
- filename: bazaarvoice-lookahead-api-openapi.yml
  format: yaml
  label: Bazaarvoice Lookahead API
  slug: bazaarvoice-lookahead-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-lookahead-api-openapi.yml
- filename: bazaarvoice-questions-api-openapi.yml
  format: yaml
  label: Bazaarvoice Questions API
  slug: bazaarvoice-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-questions-api-openapi.yml
- filename: bazaarvoice-reviews-api-openapi.yml
  format: yaml
  label: Bazaarvoice Reviews API
  slug: bazaarvoice-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-reviews-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Bazaarvoice Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Bazaarvoice secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Bazaarvoice
provider_slug: bazaarvoice
scheme_count: 3
schemes:
- description: API passkey for the Content Search API, sent as the Bv-Passkey request header. Requested and managed in the Bazaarvoice Portal API Key Management application.
  in: header
  name: Bv-Passkey
  parameter: Bv-Passkey
  sources:
  - openapi/bazaarvoice-content-search-openapi.json
  type: apiKey
- description: API passkey for the classic Conversations API, supplied as the Passkey query parameter (e.g. ?ApiVersion=5.4&Passkey={apikey}).
  docs: https://developers.bazaarvoice.com/v1.0-ConversationsAPI/docs/api-key-management
  in: query
  name: Passkey
  parameter: passkey
  type: apiKey
- description: 2-legged OAuth2 (client credentials) for the Transactions API and Response API. client_id and client_secret are issued by Bazaarvoice Support; a token is obtained from the POST /auth-v1/oauth2/token endpoint. No passkey is used for these APIs.
  docs: https://developers.bazaarvoice.com/v1.0-TransactionsAPI/docs/oauth2-2-legged
  flow: clientCredentials
  name: OAuth2ClientCredentials
  tokenUrl: https://developers.bazaarvoice.com/v1.0-TransactionsAPI/reference/post_auth-v1-oauth2-token
  type: oauth2
slug: bazaarvoice-authentication
source_filename: bazaarvoice-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/bazaarvoice-content-search-openapi.json\ndocs: https://developers.bazaarvoice.com/v1.0-ConversationsAPI/docs/api-key-management\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - clientCredentials\n  note: >-\n    Bazaarvoice uses two authentication models across its API surface. The Conversations\n    and Content Search APIs authenticate with an API passkey (the Bv-Passkey header in\n    the V2.0 Content Search API, or the Passkey query parameter in the classic\n    Conversations API). Passkeys are requested and managed in the Bazaarvoice Portal's\n    API Key Management application and must be activated by a Technical Administrator.\n    The Transactions API and Response API instead use 2-legged OAuth2 (client\n    credentials) and do not accept passkeys.\nschemes:\n- name: Bv-Passkey\n  type: apiKey\n  in: header\n  parameter: Bv-Passkey\n  description: >-\n  \
  \  API passkey for the Content Search API, sent as the Bv-Passkey request header.\n    Requested and managed in the Bazaarvoice Portal API Key Management application.\n  sources:\n  - openapi/bazaarvoice-content-search-openapi.json\n- name: Passkey\n  type: apiKey\n  in: query\n  parameter: passkey\n  description: >-\n    API passkey for the classic Conversations API, supplied as the Passkey query\n    parameter (e.g. ?ApiVersion=5.4&Passkey={apikey}).\n  docs: https://developers.bazaarvoice.com/v1.0-ConversationsAPI/docs/api-key-management\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://developers.bazaarvoice.com/v1.0-TransactionsAPI/reference/post_auth-v1-oauth2-token\n  description: >-\n    2-legged OAuth2 (client credentials) for the Transactions API and Response API.\n    client_id and client_secret are issued by Bazaarvoice Support; a token is obtained\n    from the POST /auth-v1/oauth2/token endpoint. No passkey is used for these\
  \ APIs.\n  docs: https://developers.bazaarvoice.com/v1.0-TransactionsAPI/docs/oauth2-2-legged\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/authentication/bazaarvoice-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Reviews
- Ratings
- User Generated Content
- Retail
- eCommerce
- Product Reviews
- Syndication
- Social Commerce
- SEO
---
