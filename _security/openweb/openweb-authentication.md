---
anonymous_access: false
api_key_in:
- body
api_specs:
- filename: openweb-export-api-openapi.yml
  format: yaml
  label: OpenWeb Export API
  slug: openweb-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-export-api-openapi.yml
- filename: openweb-top-comments-api-openapi.yml
  format: yaml
  label: OpenWeb top comments API
  slug: openweb-top-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-top-comments-api-openapi.yml
- filename: openweb-trending-articles-api-openapi.yml
  format: yaml
  label: OpenWeb trending articles API
  slug: openweb-trending-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-trending-articles-api-openapi.yml
- filename: openweb-article-api-openapi.yml
  format: yaml
  label: OpenWeb Article API
  slug: openweb-article-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-article-api-openapi.yml
- filename: openweb-comment-api-openapi.yml
  format: yaml
  label: OpenWeb Comment API
  slug: openweb-comment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-comment-api-openapi.yml
- filename: openweb-live-blog-api-openapi.yml
  format: yaml
  label: OpenWeb live blog API
  slug: openweb-live-blog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-live-blog-api-openapi.yml
- filename: openweb-moderation-policy-api-openapi.yml
  format: yaml
  label: OpenWeb moderation policy API
  slug: openweb-moderation-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-moderation-policy-api-openapi.yml
- filename: openweb-score-and-reviews-api-openapi.yml
  format: yaml
  label: OpenWeb score and reviews API
  slug: openweb-score-and-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-score-and-reviews-api-openapi.yml
- filename: openweb-sso-api-openapi.yml
  format: yaml
  label: OpenWeb SSO API
  slug: openweb-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-sso-api-openapi.yml
- filename: openweb-token-api-openapi.yml
  format: yaml
  label: OpenWeb Token API
  slug: openweb-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-token-api-openapi.yml
auth_types:
- http
- jwt
- sso
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Openweb Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenWeb secures its APIs with http, jwt, and sso across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OpenWeb
provider_slug: openweb
scheme_count: 4
schemes:
- bearerFormat: JWT
  credentials:
    apikey: Export/API key generated in the OpenWeb Admin Panel.
    spot_id: Unique OpenWeb identifier for your property (Spot ID).
  description: Server-to-server Publisher API auth. POST spot_id + apikey (the Export/API key from Admin Panel > Settings > Authentication Tokens) to https://api.openweb.com/v1/publisher/auth to mint a short-lived JWT, then send it as a Bearer token on subsequent Publisher API calls.
  name: PublisherApiToken
  scheme: bearer
  token_endpoint: https://api.openweb.com/v1/publisher/auth
  type: http
- description: 'End-user authentication for embedded Conversation. A codeA/codeB handshake: the OpenWeb SDK issues an SSO session id (codeA) which the publisher backend exchanges (with its secret access_token + user primary_key/user_name) for codeB to complete login.'
  docs: https://developers.openweb.com/docs/single-sign-on
  name: SSO
  type: sso
- description: 'Third-party SSO: authenticate users via an external identity provider by passing a signed JWT (ssoWithJwt).'
  docs: https://developers.openweb.com/docs/implement-third-party-single-sign-on
  name: SSOWithJWT
  type: openIdConnect
- description: Notification webhook verification. Supports an x-openweb-notification-event-webhook-token header (partner_secret_token) or RFC 7523 client_secret_jwt (HS256, ~600s expiry) to authenticate delivered events.
  docs: https://developers.openweb.com/docs/notification-webhook
  name: WebhookClientSecretJWT
  scheme: client_secret_jwt
  type: oauth2
slug: openweb-authentication
source_filename: openweb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developers.openweb.com/docs/authentication + https://developers.openweb.com/reference/post_v1-publisher-auth\ndocs: https://developers.openweb.com/docs/getting-started\nsummary:\n  types: [http, jwt, sso]\n  api_key_in: [body]\n  token_endpoint: https://api.openweb.com/v1/publisher/auth\nschemes:\n- name: PublisherApiToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Server-to-server Publisher API auth. POST spot_id + apikey (the Export/API\n    key from Admin Panel > Settings > Authentication Tokens) to\n    https://api.openweb.com/v1/publisher/auth to mint a short-lived JWT, then send\n    it as a Bearer token on subsequent Publisher API calls.\n  token_endpoint: https://api.openweb.com/v1/publisher/auth\n  credentials:\n    spot_id: Unique OpenWeb identifier for your property (Spot ID).\n    apikey: Export/API key generated in the OpenWeb Admin Panel.\n- name: SSO\n  type: sso\n  description:\
  \ >-\n    End-user authentication for embedded Conversation. A codeA/codeB handshake:\n    the OpenWeb SDK issues an SSO session id (codeA) which the publisher backend\n    exchanges (with its secret access_token + user primary_key/user_name) for\n    codeB to complete login.\n  docs: https://developers.openweb.com/docs/single-sign-on\n- name: SSOWithJWT\n  type: openIdConnect\n  description: >-\n    Third-party SSO: authenticate users via an external identity provider by\n    passing a signed JWT (ssoWithJwt).\n  docs: https://developers.openweb.com/docs/implement-third-party-single-sign-on\n- name: WebhookClientSecretJWT\n  type: oauth2\n  scheme: client_secret_jwt\n  description: >-\n    Notification webhook verification. Supports an x-openweb-notification-event-webhook-token\n    header (partner_secret_token) or RFC 7523 client_secret_jwt (HS256, ~600s\n    expiry) to authenticate delivered events.\n  docs: https://developers.openweb.com/docs/notification-webhook\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/authentication/openweb-authentication.yml
summary_line: http/jwt/sso · 4 schemes
tags:
- Company
- Consumer
- Community
- Comments
- Audience Engagement
- Publishing
- Media
- Moderation
- Identity
- SSO
- Webhook
---
