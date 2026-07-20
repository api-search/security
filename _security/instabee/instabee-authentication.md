---
api_key_in:
- header
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Instabee Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Instabee secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Instabee
provider_slug: instabee
scheme_count: 3
schemes:
- description: 'Primary API authentication. HTTP Basic with the API key as username and API secret as password, sent as Authorization: Basic base64(apiKey:apiSecret) over TLS.'
  name: basicAuth
  scheme: basic
  sources:
  - https://developer.budbee.com/
  type: http
- description: 'Optional OAuth2 client-credentials authentication for outbound Webhooks V2 callbacks. The merchant configures a token endpoint URL, client ID/secret and optional scopes in the partner portal; Budbee obtains a bearer token and sends Authorization: Bearer <access_token> on callbacks.'
  flows:
  - flow: clientCredentials
  name: webhookOAuth2
  scheme: bearer
  sources:
  - https://developer.budbee.com/
  type: oauth2
- description: Shipping-label URLs are pre-signed with query-string HMAC-SHA256 signatures (X-Budbee-Algorithm, X-Budbee-Date, X-Budbee-Expires, X-Budbee-Signature), valid for 48 hours. Parameters are already percent-encoded and must not be re-encoded.
  in: query
  name: presignedUrl
  sources:
  - https://developer.budbee.com/
  type: apiKey
slug: instabee-authentication
source_filename: instabee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.budbee.com/\ndocs: https://developer.budbee.com/\nprovider: Instabee\nproviderId: instabee\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nnotes: >-\n  Developer credentials (separate key pairs for sandbox and production) are issued by Budbee on\n  request via onboarding@budbee.com. Merchant OAuth2 for Webhooks V2 is configured in the partner\n  portal at partner.instabee.com.\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    Primary API authentication. HTTP Basic with the API key as username and API secret as password,\n    sent as Authorization: Basic base64(apiKey:apiSecret) over TLS.\n  sources:\n  - https://developer.budbee.com/\n- name: webhookOAuth2\n  type: oauth2\n  scheme: bearer\n  description: >-\n    Optional OAuth2 client-credentials authentication for outbound Webhooks V2 callbacks. The\n    merchant\
  \ configures a token endpoint URL, client ID/secret and optional scopes in the partner\n    portal; Budbee obtains a bearer token and sends Authorization: Bearer <access_token> on callbacks.\n  flows:\n  - flow: clientCredentials\n  sources:\n  - https://developer.budbee.com/\n- name: presignedUrl\n  type: apiKey\n  in: query\n  description: >-\n    Shipping-label URLs are pre-signed with query-string HMAC-SHA256 signatures (X-Budbee-Algorithm,\n    X-Budbee-Date, X-Budbee-Expires, X-Budbee-Signature), valid for 48 hours. Parameters are already\n    percent-encoded and must not be re-encoded.\n  sources:\n  - https://developer.budbee.com/\nwebhook_signature:\n  header: X-Budbee-Signature\n  algorithm: HMAC-SHA1\n  description: >-\n    Inbound webhook payloads are signed with a SHA-1 HMAC of the request body using the merchant's\n    secret API key, for integrity verification.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instabee/refs/heads/main/authentication/instabee-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Retail
- Logistics
- Last-Mile Delivery
- Shipping
- E-commerce
- Parcel Lockers
- Returns
- Nordics
---
