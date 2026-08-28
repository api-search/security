---
api_key_in: []
auth_types: []
description: ShipHawk uses a single key-based authentication scheme. There is no OAuth 2.0, no OpenID Connect, no mutual TLS and no scope surface — one API key per environment carries full account authority. Keys can be sent either as a request header or as a URL query parameter; the query-parameter form is documented by ShipHawk and is used throughout their own cURL examples, which puts credentials in server logs, browser history and referrer headers.
kind: authentication
layout: security
method: searched
name: Shiphawk Authentication
name_suffix: Authentication
oauth_flows: []
overview: ShipHawk declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ShipHawk
provider_slug: shiphawk
scheme_count: 2
schemes:
- description: Primary documented mechanism. Header name is case-insensitive in ShipHawk's examples (X-Api-Key, x-api-key and X-API-KEY all appear in the reference).
  docs: https://docs.shiphawk.com/#authentication
  example_shape: 'x-api-key: <YOUR_API_KEY>'
  id: api_key_header
  in: header
  name: X-Api-Key
  type: apiKey
- description: Documented alternative — "Pass your API Key in the X-Api-Key Header or as a param in an HTTP request." ShipHawk's own examples for the rates, shipments and unpacked-item endpoints use this form (e.g. POST /api/v4/rates?api_key=...).
  docs: https://docs.shiphawk.com/#authentication
  id: api_key_query
  in: query
  name: api_key
  risk: Credentials in the query string are recorded by proxies, CDNs, access logs and browser history. Prefer the header form.
  type: apiKey
slug: shiphawk-authentication
source_filename: shiphawk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://docs.shiphawk.com/#authentication\ndocs: https://docs.shiphawk.com/#authentication\ndescription: >-\n  ShipHawk uses a single key-based authentication scheme. There is no OAuth 2.0, no\n  OpenID Connect, no mutual TLS and no scope surface — one API key per environment\n  carries full account authority. Keys can be sent either as a request header or as a\n  URL query parameter; the query-parameter form is documented by ShipHawk and is used\n  throughout their own cURL examples, which puts credentials in server logs, browser\n  history and referrer headers.\napi_style: REST over HTTPS (HTTPS is mandatory — \"all API requests MUST be made over HTTPS\")\nschemes:\n- id: api_key_header\n  type: apiKey\n  in: header\n  name: X-Api-Key\n  description: >-\n    Primary documented mechanism. Header name is case-insensitive in ShipHawk's examples\n    (X-Api-Key, x-api-key and X-API-KEY all appear in the reference).\n  example_shape:\
  \ \"x-api-key: <YOUR_API_KEY>\"\n  docs: https://docs.shiphawk.com/#authentication\n- id: api_key_query\n  type: apiKey\n  in: query\n  name: api_key\n  description: >-\n    Documented alternative — \"Pass your API Key in the X-Api-Key Header or as a param in\n    an HTTP request.\" ShipHawk's own examples for the rates, shipments and unpacked-item\n    endpoints use this form (e.g. POST /api/v4/rates?api_key=...).\n  risk: >-\n    Credentials in the query string are recorded by proxies, CDNs, access logs and browser\n    history. Prefer the header form.\n  docs: https://docs.shiphawk.com/#authentication\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes: false\nscopes_note: >-\n  ShipHawk publishes no OAuth scope or permission reference; authorization is expressed\n  through user permission levels in the web portal, not through token scopes. No\n  scopes/ artifact is emitted (the pipeline's scopes/ recipe is OAuth-only).\nkey_management:\n  keys_per_account: 2\n  environments:\n\
  \  - name: production\n    host: https://shiphawk.com\n    api_base: https://shiphawk.com/api/v4\n  - name: sandbox\n    host: https://sandbox.shiphawk.com\n    api_base: https://sandbox.shiphawk.com/api/v4\n  cross_environment_behavior: >-\n    \"These keys are unique to their environments, and will result in authentication\n    failures (403 Forbidden) if used in the incorrect environment.\"\n  rotation_policy: not documented\n  key_prefix: not documented\n  self_service_issuance: not documented — keys are obtained through the ShipHawk account/portal\nfailure_modes:\n- status: 401\n  meaning: Unauthorized. Your authentication credentials are out of date or invalid.\n- status: 403\n  meaning: >-\n    Forbidden. You do not have permission to perform the request — also returned when a\n    sandbox key is used against production or vice versa.\n- status: 402\n  meaning: Suspended. Your account has been suspended (contact support@shiphawk.com).\nx-evidence:\n  probed: '2026-08-27'\n  url:\
  \ https://shiphawk.com/api/v4/user\n  http_status: 401\n  content_type: application/json\n  body: '{\"error\":\"401 Unauthorized\"}'\n  note: >-\n    Unauthenticated probe of the live production base confirms the documented base URL and\n    the JSON error envelope. Response headers carried x-request-id, x-release-version\n    (v2026.6.0) and x-runtime; no WWW-Authenticate and no rate-limit headers were returned.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shiphawk/refs/heads/main/authentication/shiphawk-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Shipping
- Logistics
- Transportation Management
- Warehouse Management
- Freight
- Parcel
- Fulfillment
- eCommerce
- Supply Chain
- Carriers
- Rate Shopping
- Tracking
- Webhooks
---
