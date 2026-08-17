---
api_key_in:
- query
- body
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Eligible Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eligible secures its APIs with apiKey across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Eligible
provider_slug: eligible
scheme_count: 5
schemes:
- applies_to: GET, HEAD, DELETE
  description: On GET/HEAD/DELETE the client appends the account API key to the query string as `api_key=<key>` (together with `test=true|false`). Confirmed in Eligible::request in the Ruby gem.
  in: query
  name: api_key
  parameter: api_key
  source: rubygems:eligible@3.0.3 lib/eligible.rb
  type: apiKey
- applies_to: POST, PUT
  description: On write methods the API key is merged into the JSON request body alongside `test`, rather than sent as a parameter.
  in: body
  name: api_key
  parameter: api_key
  source: rubygems:eligible@3.0.3 lib/eligible.rb
  type: apiKey
- description: 'The Ruby client additionally sets `Authorization: Bearer <api_key>` on every request. The same key value is used; this is a header carriage of the API key, not a separate OAuth token, and there is no authorization server, token endpoint, refresh flow or scope set anywhere in the client or the docs.'
  in: header
  name: authorization_bearer
  parameter: Authorization
  scheme: bearer
  source: rubygems:eligible@3.0.3 lib/eligible.rb
  type: http
- description: A short-lived alternative credential. `POST /session_tokens/create.json` mints one and `POST /session_tokens/revoke.json` destroys it; when a session_token is supplied the client does not require the account API key. Intended for browser/mobile contexts where the long-lived key must not be shipped.
  in: body
  name: session_token
  parameter: session_token
  source: rubygems:eligible@3.0.3 lib/eligible/session_token.rb
  type: apiKey
- description: 'A separate, non-authenticating identifier. Eligible''s own FAQ is explicit: "The publishable key is used in certain libs for identifying the customer, but the API key is used for authentication across all the API. In all cases, use the API key unless prompted for the publishable key." Sending it where the API key is expected is the documented cause of a 401.'
  in: body
  name: publishable_key
  parameter: publishable_key
  source: https://eligible.com/community/technical-features-faq/
  type: apiKey
slug: eligible-authentication
source_filename: eligible-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: >-\n  https://eligible.com/community/technical-features-faq/ (Eligible's published\n  Technical & Features FAQ) cross-read against the request layer of Eligible's own\n  first-party clients: rubygems.org eligible 3.0.3 (lib/eligible.rb) and\n  registry.npmjs.org eligible-node 1.2.9 (lib/http/client.js, lib/http/config.js).\ndocs: https://eligible.com/community/technical-features-faq/\nnote: >-\n  DERIVED FROM FIRST-PARTY CLIENT SOURCE, NOT FROM AN OPENAPI. Eligible publishes no\n  machine-readable specification, and its API reference sits behind an account login\n  (https://eligible.com/docs serves a \"Sign In\" page). Everything below is read out\n  of the vendor's own published SDKs and its own public FAQ, so it describes the\n  scheme Eligible actually implements; it is not a securityScheme block harvested\n  from a spec, and it is not a guess.\nsummary:\n  types: [apiKey]\n  api_key_in: [query, body, header]\n  oauth2_flows:\
  \ []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  bearer_token: true\nschemes:\n  - name: api_key\n    type: apiKey\n    in: query\n    parameter: api_key\n    applies_to: GET, HEAD, DELETE\n    description: >-\n      On GET/HEAD/DELETE the client appends the account API key to the query string\n      as `api_key=<key>` (together with `test=true|false`). Confirmed in\n      Eligible::request in the Ruby gem.\n    source: rubygems:eligible@3.0.3 lib/eligible.rb\n  - name: api_key\n    type: apiKey\n    in: body\n    parameter: api_key\n    applies_to: POST, PUT\n    description: >-\n      On write methods the API key is merged into the JSON request body alongside\n      `test`, rather than sent as a parameter.\n    source: rubygems:eligible@3.0.3 lib/eligible.rb\n  - name: authorization_bearer\n    type: http\n    scheme: bearer\n    in: header\n    parameter: Authorization\n    description: >-\n      The Ruby client additionally sets `Authorization: Bearer <api_key>`\
  \ on every\n      request. The same key value is used; this is a header carriage of the API key,\n      not a separate OAuth token, and there is no authorization server, token\n      endpoint, refresh flow or scope set anywhere in the client or the docs.\n    source: rubygems:eligible@3.0.3 lib/eligible.rb\n  - name: session_token\n    type: apiKey\n    in: body\n    parameter: session_token\n    description: >-\n      A short-lived alternative credential. `POST /session_tokens/create.json` mints\n      one and `POST /session_tokens/revoke.json` destroys it; when a session_token is\n      supplied the client does not require the account API key. Intended for\n      browser/mobile contexts where the long-lived key must not be shipped.\n    source: rubygems:eligible@3.0.3 lib/eligible/session_token.rb\n  - name: publishable_key\n    type: apiKey\n    in: body\n    parameter: publishable_key\n    description: >-\n      A separate, non-authenticating identifier. Eligible's own FAQ is explicit:\
  \ \"The\n      publishable key is used in certain libs for identifying the customer, but the\n      API key is used for authentication across all the API. In all cases, use the\n      API key unless prompted for the publishable key.\" Sending it where the API key\n      is expected is the documented cause of a 401.\n    source: https://eligible.com/community/technical-features-faq/\nkey_management:\n  issued_from: https://account.eligible.com/ (\"Admin > API keys\")\n  environments: [live, staging, sandbox]\n  rotation: >-\n    Keys are reset by the account holder from the admin console; Eligible documents\n    no programmatic key-rotation endpoint.\n  note: >-\n    Three distinct keys per account, one per environment. The environment is\n    additionally selected per request by the `test` parameter, which every client\n    sends on every call.\ntransport:\n  tls: required\n  certificate_pinning: true\n  pinning_note: >-\n    Unusually, both first-party clients PIN the SHA-1 fingerprint\
  \ of the\n    gds.eligibleapi.com leaf certificate and refuse to connect on a mismatch (Ruby:\n    Eligible.fingerprints, 7 digests; Node: FINGERPRINTS, 5 digests). This is why the\n    SDKs ship a new version roughly every January — the pinned certificate rotates\n    and an un-upgraded client stops working. It is a real operational constraint for\n    any consumer and is not documented anywhere on the public site.\n  observed_response_headers:\n    strict-transport-security: max-age=63072000; includeSubDomains; preload\n    x-frame-options: DENY\n    x-content-type-options: nosniff\n    referrer-policy: strict-origin-when-cross-origin\n    cross-origin-opener-policy: same-origin\n  observed_on: https://gds.eligibleapi.com/v1.5/payers.json\nfailure_mode:\n  status: 401\n  content_type: application/json\n  body: Could not authenticate you. Please re-try with a valid API key.\n  probed: '2026-08-14'\n  note: >-\n    Observed anonymously. The body is a bare string served under an\n    application/json\
  \ content type, not a JSON object — see errors/.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eligible/refs/heads/main/authentication/eligible-authentication.yml
summary_line: apiKey · 5 schemes
tags:
- Billing
- Eligibility
- Healthcare
- Insurance
- Claims
---
