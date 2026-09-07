---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'The 9flats API v1 authentication model, read from 9flats'' OWN published client library (github.com/9flats/nineflats-api) rather than from documentation — the documentation site the gem links to, http://9flats.github.com/api_docs/, now returns 404, so the provider''s source code is the only first-party statement of the auth model still reachable. No auth page, no OpenAPI securitySchemes and no OAuth discovery document were retrievable: every path on www.9flats.com, 9flats.com and api.9flats.com is behind a Cloudflare managed challenge (403).'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: 9Flats Authentication
name_suffix: Authentication
oauth_flows: []
overview: 9flats declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: 9flats
provider_slug: 9flats
scheme_count: 2
schemes:
- credentials:
  - name: api_key
    role: OAuth consumer key
  - name: api_secret
    role: OAuth consumer secret
  evidence: 'client.rb constructs ::OAuth::Consumer.new(api_key, api_secret, site: "http://www.9flats.com", scheme: :header, http_method: :post) and exposes request_token(callback_url) -> get_request_token(oauth_callback: ...) and exchange_access_token(request_token, verifier) -> get_access_token(oauth_verifier: ...). The gemspec declares a runtime dependency on the `oauth` gem.'
  flow:
  - Obtain a request token with an oauth_callback.
  - Send the user to 9flats to authorize.
  - Exchange the request token plus oauth_verifier for an access token.
  id: oauth1
  in: header
  label: OAuth 1.0a (three-legged)
  note: OAuth 1.0a, not OAuth 2.0 — there is no token endpoint, no scopes, no refresh token and no OpenID Connect surface, so scopes/ is deliberately not emitted for this provider.
  optional_for:
  - GET /api/v1/places/{slug}
  - GET /api/v1/users/{user_id}
  required_for:
  - GET /api/v1/users/{user_id}/bookings
  signature_transport: Authorization header (scheme :header)
  type: oauth1
- evidence: 'Every request in requests.rb appends QueryStringNormalizer.normalize({client_id: consumer.key}) to the path, e.g. GET /api/v1/places/{slug}?client_id=...'
  id: client_id
  in: query
  label: Consumer key echoed as a client_id query parameter
  name: client_id
  note: This is the same value as the OAuth consumer key, carried a second time in the query string. Read-only endpoints are called with the unauthenticated consumer (consumer.request) and this parameter; only user bookings require an access token.
  type: apiKey
slug: 9flats-authentication
source_filename: 9flats-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://raw.githubusercontent.com/9flats/nineflats-api/master/lib/nineflats-api/client.rb,\n  https://raw.githubusercontent.com/9flats/nineflats-api/master/lib/nineflats-api/requests.rb,\n  https://raw.githubusercontent.com/9flats/nineflats-api/master/nineflats-api.gemspec\ndescription: >-\n  The 9flats API v1 authentication model, read from 9flats' OWN published client\n  library (github.com/9flats/nineflats-api) rather than from documentation — the\n  documentation site the gem links to, http://9flats.github.com/api_docs/, now\n  returns 404, so the provider's source code is the only first-party statement of\n  the auth model still reachable. No auth page, no OpenAPI securitySchemes and no\n  OAuth discovery document were retrievable: every path on www.9flats.com,\n  9flats.com and api.9flats.com is behind a Cloudflare managed challenge (403).\nschemes:\n  - id: oauth1\n    type: oauth1\n    label: OAuth 1.0a (three-legged)\n\
  \    in: header\n    evidence: >-\n      client.rb constructs ::OAuth::Consumer.new(api_key, api_secret, site:\n      \"http://www.9flats.com\", scheme: :header, http_method: :post) and exposes\n      request_token(callback_url) -> get_request_token(oauth_callback: ...) and\n      exchange_access_token(request_token, verifier) ->\n      get_access_token(oauth_verifier: ...). The gemspec declares a runtime\n      dependency on the `oauth` gem.\n    credentials:\n      - name: api_key\n        role: OAuth consumer key\n      - name: api_secret\n        role: OAuth consumer secret\n    flow:\n      - Obtain a request token with an oauth_callback.\n      - Send the user to 9flats to authorize.\n      - Exchange the request token plus oauth_verifier for an access token.\n    signature_transport: Authorization header (scheme :header)\n    required_for:\n      - GET /api/v1/users/{user_id}/bookings\n    optional_for:\n      - GET /api/v1/places/{slug}\n      - GET /api/v1/users/{user_id}\n  \
  \  note: >-\n      OAuth 1.0a, not OAuth 2.0 — there is no token endpoint, no scopes, no\n      refresh token and no OpenID Connect surface, so scopes/ is deliberately not\n      emitted for this provider.\n  - id: client_id\n    type: apiKey\n    in: query\n    name: client_id\n    label: Consumer key echoed as a client_id query parameter\n    evidence: >-\n      Every request in requests.rb appends\n      QueryStringNormalizer.normalize({client_id: consumer.key}) to the path, e.g.\n      GET /api/v1/places/{slug}?client_id=...\n    note: >-\n      This is the same value as the OAuth consumer key, carried a second time in\n      the query string. Read-only endpoints are called with the unauthenticated\n      consumer (consumer.request) and this parameter; only user bookings require\n      an access token.\nunauthenticated_access:\n  available: true\n  note: >-\n    Search, place detail, photos, prices, reviews, calendar, user profile and\n    user favourites are fetched through consumer.request\
  \ without an access token\n    — signed with the consumer credentials only. A client_id is still required,\n    so there is no anonymous surface.\nauthorization_gate:\n  evidence: >-\n    requests.rb raises Nineflats::NotAuthenticatedException(\"User is not\n    authenticated yet!\") before calling /api/v1/users/{id}/bookings when\n    Client.client.authorized? is false.\nverification:\n  live_probe_attempted: true\n  live_probe_result: >-\n    Could not verify against the running service. GET https://www.9flats.com/api/v1/places\n    returned 403 with cf-mitigated: challenge on 2026-09-05, as did every other\n    path on every 9flats host.\n  caveat: >-\n    This profile describes API v1 as of the last release of the provider's SDK\n    (0.0.9, 2011-11-07). A v3 surface existed at https://www.9flats.com/api/v3/places/\n    per the provider's own (now removed) api_docs site; its auth model is unknown\n    and is NOT asserted here.\ncontact: api@9flats.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/9flats/refs/heads/main/authentication/9flats-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Travel
- Hospitality
- Vacation Rentals
- Short-Term Rental
- Accommodation
- Marketplace
- Booking
- Europe
---
