---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: The Ticket Fairy Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Ticket Fairy declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: The Ticket Fairy
provider_slug: the-ticket-fairy
scheme_count: 3
schemes:
- authorize_endpoint: https://www.ticketfairy.com/api/v1/oauth/authorize-rn
  client_credentials_note: The authorize call is made as `?client_id=<CLIENT_ID>` with a client_secret held in the SDK. This is a confidential-client pattern used from a public (mobile) client.
  header: 'Authorization: Bearer <access_token>'
  id: oauth2
  password_reset_endpoint: https://www.ticketfairy.com/api/v1/oauth/restore-password-rn
  refresh: The token response carries a refresh_token and the client persists it; there is no published refresh endpoint or token lifetime. Rotation semantics are undocumented.
  register_endpoint: https://www.ticketfairy.com/api/v1/oauth/register-rn
  returns:
  - access_token
  - refresh_token
  - token_type
  - scope
  scope_note: The token response includes a `scope` field which the client stores, but no scope reference, no scope list and no consent screen are published anywhere. Because the scope vocabulary is unknown, no scopes/ artifact is written — an empty or invented scope list would be worse than the honest absence.
  scopes_documented: false
  status: observed
  token_endpoint: https://www.ticketfairy.com/api/v1/oauth/access_token
  token_type: Bearer
  type: oauth2
- id: guest
  in: header
  name: Authorization-Guest
  note: A second, parallel token channel for unauthenticated ticket buyers. The API mints the guest token and returns it in the `authorization-guest` RESPONSE header; the client echoes it back on subsequent requests. It is the mechanism that lets a fan hold a cart and complete checkout without creating an account. Undocumented publicly, and confirmed accepted by the live API — `authorization-guest` is listed in Access-Control-Allow-Headers on every /api/ response.
  status: observed
  type: apiKey
- id: none
  note: 'A subset of the API is genuinely anonymous and needs no credential at all — confirmed live: GET https://www.ticketfairy.com/api/countries/list returns 200 application/json with no Authorization header, and GET https://www.theticketfairy.com/api/public/filtered-events returns 200 for a brand or venue filter. This public read surface is what the company''s own WordPress plugin consumes.'
  status: observed
  type: none
slug: the-ticket-fairy-authentication
source_filename: the-ticket-fairy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: >-\n  tf-checkout-react-native@1.0.47 (npm, published by the `theticketfairy` npm account) —\n  src/api/Constants.ts and src/api/ApiClient.ts; corroborated by live CORS preflight on\n  https://www.ticketfairy.com/api/v1/cart/ (2026-08-13)\nnote: >-\n  DERIVED, NOT PUBLISHED. The Ticket Fairy publishes no authentication documentation, no developer\n  portal and no OpenAPI. Everything below is read out of the company's OWN first-party client\n  library on npm and confirmed against the live API's CORS preflight, which enumerates exactly\n  which Authorization headers the origin accepts. No credential values are reproduced here: the\n  React Native library ships a hard-coded checkout client_id/client_secret pair in\n  src/api/Constants.ts, which is itself a finding (a shared public client secret shipped inside a\n  distributed mobile bundle) but is not repeated in this artifact.\napi: The Ticket Fairy REST API\nbase_url: https://www.ticketfairy.com/api\n\
  schemes:\n- id: oauth2\n  type: oauth2\n  status: observed\n  token_endpoint: https://www.ticketfairy.com/api/v1/oauth/access_token\n  authorize_endpoint: https://www.ticketfairy.com/api/v1/oauth/authorize-rn\n  register_endpoint: https://www.ticketfairy.com/api/v1/oauth/register-rn\n  password_reset_endpoint: https://www.ticketfairy.com/api/v1/oauth/restore-password-rn\n  token_type: Bearer\n  header: 'Authorization: Bearer <access_token>'\n  returns:\n  - access_token\n  - refresh_token\n  - token_type\n  - scope\n  refresh: >-\n    The token response carries a refresh_token and the client persists it; there is no published\n    refresh endpoint or token lifetime. Rotation semantics are undocumented.\n  scopes_documented: false\n  scope_note: >-\n    The token response includes a `scope` field which the client stores, but no scope reference,\n    no scope list and no consent screen are published anywhere. Because the scope vocabulary is\n    unknown, no scopes/ artifact is written —\
  \ an empty or invented scope list would be worse than\n    the honest absence.\n  client_credentials_note: >-\n    The authorize call is made as `?client_id=<CLIENT_ID>` with a client_secret held in the SDK.\n    This is a confidential-client pattern used from a public (mobile) client.\n- id: guest\n  type: apiKey\n  in: header\n  name: Authorization-Guest\n  status: observed\n  note: >-\n    A second, parallel token channel for unauthenticated ticket buyers. The API mints the guest\n    token and returns it in the `authorization-guest` RESPONSE header; the client echoes it back\n    on subsequent requests. It is the mechanism that lets a fan hold a cart and complete checkout\n    without creating an account. Undocumented publicly, and confirmed accepted by the live API —\n    `authorization-guest` is listed in Access-Control-Allow-Headers on every /api/ response.\n- id: none\n  type: none\n  status: observed\n  note: >-\n    A subset of the API is genuinely anonymous and needs no credential\
  \ at all — confirmed live:\n    GET https://www.ticketfairy.com/api/countries/list returns 200 application/json with no\n    Authorization header, and GET https://www.theticketfairy.com/api/public/filtered-events\n    returns 200 for a brand or venue filter. This public read surface is what the company's own\n    WordPress plugin consumes.\nmedia_types:\n  request: application/vnd.api+json\n  response: application/vnd.api+json\n  note: >-\n    The client sets JSON:API media types by default and unwraps `data.data.attributes.*` on\n    responses, so the authenticated surface is JSON:API-flavored. The anonymous public endpoints\n    answer plain application/json with a flat {data, success, error, message, status} envelope —\n    the two surfaces do not share an envelope.\naccepted_auth_headers_live:\n  source: CORS preflight, https://www.ticketfairy.com/api/v1/cart/, 2026-08-13\n  headers:\n  - authorization\n  - authorization-guest\n  - x-tf-ecommerce\n  - x-tf-context\n  - promotion-code\n\
  \  - promotion-event\n  - referrer-id\n  - device-info\n  - referer-url\n  - additional-cookies\n  - phpr-remote-event\n  - idempotency-key\ndocs: null\ndocs_note: >-\n  No public authentication page exists. Searched ticketfairy.com and theticketfairy.com for\n  /developers, /api, /api-documentation, /docs — all 404.\ngaps:\n- No published OAuth scope reference, despite the token response carrying a `scope` field.\n- No documented token lifetime, refresh flow, or revocation endpoint.\n- No /.well-known/oauth-authorization-server or /.well-known/openid-configuration (both 404).\n- A client_secret is shipped inside a public npm package and therefore inside every app that\n  bundles it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-ticket-fairy/refs/heads/main/authentication/the-ticket-fairy-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Ticketing
- Events
- Event Management
- Payments
- Marketing
- Entertainment
- Checkout
- Festivals
- Live Events
- Embedded Commerce
- Access Control
---
