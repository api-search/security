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
- filename: bazaarvoice-conversations-display-openapi.yml
  format: yaml
  label: Bazaarvoice Conversations Display API
  slug: bazaarvoice-conversations-display-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-conversations-display-openapi.yml
- filename: bazaarvoice-conversations-submission-openapi.yml
  format: yaml
  label: Bazaarvoice Conversations Submission API
  slug: bazaarvoice-conversations-submission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-conversations-submission-openapi.yml
- filename: bazaarvoice-response-openapi.yml
  format: yaml
  label: Bazaarvoice Response API
  slug: bazaarvoice-response-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-response-openapi.yml
- filename: bazaarvoice-response-count-openapi.yml
  format: yaml
  label: Bazaarvoice Response Count API
  slug: bazaarvoice-response-count-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-response-count-openapi.yml
- filename: bazaarvoice-notifications-subscriptions-openapi.yml
  format: yaml
  label: Bazaarvoice Notifications Subscriptions API
  slug: bazaarvoice-notifications-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-notifications-subscriptions-openapi.yml
- filename: bazaarvoice-transactions-openapi.yml
  format: yaml
  label: Bazaarvoice Transactions API
  slug: bazaarvoice-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-transactions-openapi.yml
- filename: bazaarvoice-product-sentiment-openapi.yml
  format: yaml
  label: Bazaarvoice Product Sentiment API
  slug: bazaarvoice-product-sentiment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-product-sentiment-openapi.yml
- filename: bazaarvoice-social-commerce-media-openapi.yml
  format: yaml
  label: Bazaarvoice Social Commerce Display (Media) API
  slug: bazaarvoice-social-commerce-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-social-commerce-media-openapi.yml
- filename: bazaarvoice-authentic-discovery-openapi.yml
  format: yaml
  label: Bazaarvoice Authentic Discovery API
  slug: bazaarvoice-authentic-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-authentic-discovery-openapi.yml
- filename: bazaarvoice-displayable-content-export-openapi.yml
  format: yaml
  label: Bazaarvoice Displayable Content Export
  slug: bazaarvoice-displayable-content-export
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-displayable-content-export-openapi.yml
- filename: bazaarvoice-product-sentiment-export-openapi.yml
  format: yaml
  label: Bazaarvoice Product Sentiment Export
  slug: bazaarvoice-product-sentiment-export
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-product-sentiment-export-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Bazaarvoice Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Bazaarvoice secures its APIs with apiKey, http, and oauth2 across 7 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Bazaarvoice
provider_slug: bazaarvoice
scheme_count: 7
schemes:
- description: API passkey for the V2.0 Content Search API, sent as the Bv-Passkey request header.
  in: header
  name: Bv-Passkey
  parameter: Bv-Passkey
  sources:
  - openapi/_original/bazaarvoice-content-search-openapi.json
  type: apiKey
- description: Authentic Discovery API key, sent as the Bv-passkey request header on GET /clients/{clientId}/ugc (note the lower-case "p" - the Authentic Discovery document spells the header differently from the Content Search document).
  in: header
  name: Bv-passkey
  parameter: Bv-passkey
  sources:
  - openapi/_original/bazaarvoice-authentic-discovery-openapi.json
  type: apiKey
- description: API passkey for the classic Conversations API, supplied as the Passkey query parameter (e.g. ?ApiVersion=5.4&Passkey={apikey}).
  docs: https://developers.bazaarvoice.com/v1.0-ConversationsAPI/docs/api-key-management
  in: query
  name: Passkey
  parameter: passkey
  type: apiKey
- description: Notifications Subscriptions API passkey, supplied as the passkey query parameter.
  in: query
  name: apiKey
  parameter: passkey
  sources:
  - openapi/_original/bazaarvoice-notifications-subscriptions-openapi.json
  type: apiKey
- description: Bearer access token for the Transactions API, obtained from the 2-legged OAuth2 client-credentials endpoint. client_id and client_secret are issued by Bazaarvoice Support.
  docs: https://developers.bazaarvoice.com/v1.0-TransactionsAPI/docs/oauth2-2-legged
  name: accessToken
  scheme: bearer
  sources:
  - openapi/_original/bazaarvoice-transactions-openapi.json
  type: http
- description: Bearer access token for the Response API. The spec's own scheme description documents a two-part login against identity(-stg).portal.bazaarvoice.com/api/v1/oauth2/login followed by a token exchange.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/_original/bazaarvoice-response-openapi.json
  - openapi/_original/bazaarvoice-response-count-openapi.json
  type: http
- description: API key header for the Social Commerce Display (Media) API. Bazaarvoice's own Social Commerce docs state that all endpoints are served from edge.curalate.com - Curalate is the visual-commerce company Bazaarvoice acquired, and the product still runs on that platform and its key header.
  in: header
  name: ApiKey
  parameter: X-Curalate-Api-Key
  sources:
  - openapi/_original/bazaarvoice-social-commerce-media-openapi.json
  type: apiKey
slug: bazaarvoice-authentication
source_filename: bazaarvoice-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource:\n- openapi/_original/\n- https://developers.bazaarvoice.com/v1.0-ConversationsAPI/docs/api-key-management\n- https://developers.bazaarvoice.com/v1.0-TransactionsAPI/docs/oauth2-2-legged\n- https://developers.bazaarvoice.com/v1.0-ConversationsAPI/docs/platform-api-concepts\ndocs: https://developers.bazaarvoice.com/v1.0-ConversationsAPI/docs/api-key-management\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  http_schemes:\n  - bearer\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\n  note: >-\n    Bazaarvoice runs three distinct authentication models across its API estate, and which one\n    applies depends entirely on which product you are calling. (1) An API PASSKEY - the Bv-Passkey\n    header on the Content Search and Authentic Discovery APIs, or a Passkey query parameter on the\n    classic Conversations and Notifications Subscriptions APIs. Passkeys are requested\
  \ and managed\n    in the Bazaarvoice Portal API Key Management application and must be activated by a Technical\n    Administrator. (2) HTTP BEARER tokens obtained from OAuth2 - the Transactions API uses a\n    2-legged client-credentials flow against POST /auth-v1/oauth2/token, while the Response and\n    Privacy APIs also document a 3-legged flow through identity.portal.bazaarvoice.com. (3) A\n    separate X-Curalate-Api-Key header on the Social Commerce Display (Media) API, which runs on\n    the Curalate platform Bazaarvoice acquired.\nschemes:\n- name: Bv-Passkey\n  type: apiKey\n  in: header\n  parameter: Bv-Passkey\n  description: >-\n    API passkey for the V2.0 Content Search API, sent as the Bv-Passkey request header.\n  sources:\n  - openapi/_original/bazaarvoice-content-search-openapi.json\n- name: Bv-passkey\n  type: apiKey\n  in: header\n  parameter: Bv-passkey\n  description: >-\n    Authentic Discovery API key, sent as the Bv-passkey request header on\n    GET /clients/{clientId}/ugc\
  \ (note the lower-case \"p\" - the Authentic Discovery document spells\n    the header differently from the Content Search document).\n  sources:\n  - openapi/_original/bazaarvoice-authentic-discovery-openapi.json\n- name: Passkey\n  type: apiKey\n  in: query\n  parameter: passkey\n  description: >-\n    API passkey for the classic Conversations API, supplied as the Passkey query parameter\n    (e.g. ?ApiVersion=5.4&Passkey={apikey}).\n  docs: https://developers.bazaarvoice.com/v1.0-ConversationsAPI/docs/api-key-management\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: passkey\n  description: Notifications Subscriptions API passkey, supplied as the passkey query parameter.\n  sources:\n  - openapi/_original/bazaarvoice-notifications-subscriptions-openapi.json\n- name: accessToken\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer access token for the Transactions API, obtained from the 2-legged OAuth2\n    client-credentials endpoint. client_id and client_secret\
  \ are issued by Bazaarvoice Support.\n  docs: https://developers.bazaarvoice.com/v1.0-TransactionsAPI/docs/oauth2-2-legged\n  sources:\n  - openapi/_original/bazaarvoice-transactions-openapi.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer access token for the Response API. The spec's own scheme description documents a\n    two-part login against identity(-stg).portal.bazaarvoice.com/api/v1/oauth2/login followed by a\n    token exchange.\n  sources:\n  - openapi/_original/bazaarvoice-response-openapi.json\n  - openapi/_original/bazaarvoice-response-count-openapi.json\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-Curalate-Api-Key\n  description: >-\n    API key header for the Social Commerce Display (Media) API. Bazaarvoice's own Social Commerce\n    docs state that all endpoints are served from edge.curalate.com - Curalate is the visual-commerce\n    company Bazaarvoice acquired, and the product still runs on that platform and its\
  \ key header.\n  sources:\n  - openapi/_original/bazaarvoice-social-commerce-media-openapi.json\noauth2:\n  flows:\n  - flow: clientCredentials\n    name: 2-legged\n    token_endpoint_docs: https://developers.bazaarvoice.com/v1.0-TransactionsAPI/reference/post_auth-v1-oauth2-token\n    applies_to: [Transactions API, Privacy API]\n    docs: https://developers.bazaarvoice.com/v1.0-TransactionsAPI/docs/oauth2-2-legged\n  - flow: authorizationCode\n    name: 3-legged\n    login_endpoint: https://identity.portal.bazaarvoice.com/api/v1/oauth2/login\n    applies_to: [Privacy API, Response API]\n    docs: https://developers.bazaarvoice.com/v1.0-PrivacyAPI/reference/privacy-post-auth-v1-oauth2-token-reference\n  scopes_published: false\nkey_management:\n  portal: https://portal.bazaarvoice.com\n  docs: https://developers.bazaarvoice.com/v1.0-ConversationsAPI/docs/api-key-management\n  detail: >-\n    Keys are requested per client through the API Key Management application in the Bazaarvoice\n \
  \   Portal; a Technical Administrator must activate a key before it will authenticate. The portal\n    also shows each key's status and rate-limit allotment.\nauthor_authentication:\n  detail: >-\n    Distinct from API authentication: content SUBMISSION additionally requires an author identity,\n    either BV-mastered (Bazaarvoice hosts the user account) or client-mastered (the client passes a\n    signed user id). Device fingerprinting via iovation is documented as part of the submission\n    anti-fraud path.\n  docs:\n  - https://developers.bazaarvoice.com/v1.0-ConversationsAPI/docs/bv-mastered-authentication\n  - https://developers.bazaarvoice.com/v1.0-ConversationsAPI/docs/client-mastered-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/authentication/bazaarvoice-authentication.yml
summary_line: apiKey/http/oauth2 · 7 schemes
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
