---
api_key_in:
- header
auth_types:
- oauth2
- http
- apiKey
description: Authentication model for the Bread Pay developer surface, captured from the published API-access documentation (no OpenAPI securitySchemes were available to derive from). The next-generation BreadPay Platform API uses OAuth 2.0; the legacy sandbox/servicing API uses HTTP Basic plus a client token header.
kind: authentication
layout: security
method: searched
name: Bread Financial Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Bread Financial secures its APIs with oauth2, http, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Bread Financial
provider_slug: bread-financial
scheme_count: 3
schemes:
- detail: BreadPay Platform APIs use the OAuth 2.0 Client Credentials Flow for server-to-server (2-legged) interactions. Client credentials are sent using HTTP Basic Authentication (Base64 of client_id:client_secret) to the authorization server, which returns a JWT access token. Credentials are issued from the Bread Merchant Portal / by the Bread partnership team.
  flow: clientCredentials
  name: BreadPay OAuth 2.0 (client credentials)
  source: https://platform-docs.breadpayments.com/bread-developers/docs/api-access
  token_format: JWT
  type: oauth2
- detail: The partner sandbox / enterprise servicing API requires HTTP Basic Auth (Base64 of client_id:client_secret) in the Authorization header PLUS a separate client_token header (alphanumeric, up to 50 chars) designated by Bread Financial. Requests must also originate from an allow-listed IP range.
  name: Sandbox Basic Auth + client token
  scheme: basic
  source: https://platform-docs.breadpayments.com/bread-onboarding/docs/sandbox-access
  type: http
- detail: Browser SDK and Bread Classic checkout flows are initialized with a merchant integrationKey (public) that identifies the merchant program; server-side Classic calls additionally use an API key + shared secret.
  in: header
  name: Merchant integration key
  source: https://docs.breadpayments.com/bread-classic/reference/getting-started-with-your-api
  type: apiKey
slug: bread-financial-authentication
source_filename: bread-financial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://platform-docs.breadpayments.com/bread-developers/docs/api-access\ndocs:\n- https://platform-docs.breadpayments.com/bread-developers/docs/api-access\n- https://docs.breadpayments.com/bread-classic/reference/getting-started-with-your-api\ndescription: >-\n  Authentication model for the Bread Pay developer surface, captured from the\n  published API-access documentation (no OpenAPI securitySchemes were available\n  to derive from). The next-generation BreadPay Platform API uses OAuth 2.0; the\n  legacy sandbox/servicing API uses HTTP Basic plus a client token header.\nsummary:\n  types: [oauth2, http, apiKey]\n  oauth2_flows: [clientCredentials]\n  api_key_in: [header]\nschemes:\n- name: BreadPay OAuth 2.0 (client credentials)\n  type: oauth2\n  flow: clientCredentials\n  token_format: JWT\n  detail: >-\n    BreadPay Platform APIs use the OAuth 2.0 Client Credentials Flow for\n    server-to-server (2-legged) interactions.\
  \ Client credentials are sent using\n    HTTP Basic Authentication (Base64 of client_id:client_secret) to the\n    authorization server, which returns a JWT access token. Credentials are\n    issued from the Bread Merchant Portal / by the Bread partnership team.\n  source: https://platform-docs.breadpayments.com/bread-developers/docs/api-access\n- name: Sandbox Basic Auth + client token\n  type: http\n  scheme: basic\n  detail: >-\n    The partner sandbox / enterprise servicing API requires HTTP Basic Auth\n    (Base64 of client_id:client_secret) in the Authorization header PLUS a\n    separate client_token header (alphanumeric, up to 50 chars) designated by\n    Bread Financial. Requests must also originate from an allow-listed IP range.\n  source: https://platform-docs.breadpayments.com/bread-onboarding/docs/sandbox-access\n- name: Merchant integration key\n  type: apiKey\n  in: header\n  detail: >-\n    Browser SDK and Bread Classic checkout flows are initialized with a merchant\n \
  \   integrationKey (public) that identifies the merchant program; server-side\n    Classic calls additionally use an API key + shared secret.\n  source: https://docs.breadpayments.com/bread-classic/reference/getting-started-with-your-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bread-financial/refs/heads/main/authentication/bread-financial-authentication.yml
summary_line: oauth2/http/apiKey · 3 schemes
tags:
- Company
- Fintech
- Payments
- Buy Now Pay Later
- Lending
- Consumer Finance
- Point of Sale
- Ecommerce
---
