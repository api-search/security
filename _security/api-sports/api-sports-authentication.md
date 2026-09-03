---
api_key_in: []
auth_types: []
description: Authentication profile for the API-Sports family of sports-data APIs. API-Sports publishes no OpenAPI, so this profile was established by probing the live edge with candidate header names and recording which ones the gateway recognises. Two header names are accepted, corresponding to the provider's two distribution channels (direct subscription and the RapidAPI marketplace); every other credential shape is rejected at the edge before routing.
kind: authentication
layout: security
method: probed
name: Api Sports Authentication
name_suffix: Authentication
oauth_flows: []
overview: API-Sports declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: API-Sports
provider_slug: api-sports
scheme_count: 3
schemes:
- channel: direct
  description: API key issued from the API-Sports dashboard (dashboard.api-football.com) and used when calling the sport hosts directly, e.g. v3.football.api-sports.io. One key works across every sport API the account is subscribed to.
  evidence:
    body_excerpt: '{"get":"status","parameters":[],"errors":{"token":"Error/Missing application key. Go to https://www.api-football.com/documentation-v3 to learn how to get your API application key."},"results":0,...}'
    http_status: 200
    reading: The header name is recognised — the request passes the edge (HTTP 200) and is rejected by the application's own token check, which names the documentation page.
    request_header: 'x-apisports-key: <placeholder>'
    url: https://v3.football.api-sports.io/status
  id: apisports-key
  in: header
  name: x-apisports-key
  type: apiKey
  verified: probed
- channel: marketplace
  companion_header: x-rapidapi-host
  description: RapidAPI marketplace key, used with the companion x-rapidapi-host header when calling through api-football-v1.p.rapidapi.com and the sibling RapidAPI hosts. Billing and quota are managed by RapidAPI rather than by API-Sports.
  evidence:
    http_status: 200
    reading: Also recognised at the direct host — the edge accepts either key header name and defers to the application token check.
    request_header: 'x-rapidapi-key: <placeholder>'
    url: https://v3.football.api-sports.io/status
  id: rapidapi-key
  in: header
  name: x-rapidapi-key
  type: apiKey
  verified: probed
- channel: marketplace
  evidence:
    body: '{"message":"Invalid API key. Go to https://docs.rapidapi.com/docs/keys for more info."}'
    http_status: 401
    reading: The marketplace gateway returns a conventional HTTP 401 with its own error envelope — a different failure shape from the direct hosts.
    url: https://api-football-v1.p.rapidapi.com/v3/status
  host: api-football-v1.p.rapidapi.com
  id: rapidapi-gateway
  in: header
  name: x-rapidapi-key
  type: apiKey
  verified: probed
slug: api-sports-authentication
source_filename: api-sports-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: >-\n  Live unauthenticated header probes against https://v3.football.api-sports.io/status\n  on 2026-09-02, cross-read against https://www.api-football.com/documentation-v3\n  (the URL the API's own error body names).\nspecification: API Evangelist Authentication Profile\nspecificationVersion: '0.1'\nprovider: API-Sports\nproviderId: api-sports\ndescription: >-\n  Authentication profile for the API-Sports family of sports-data APIs. API-Sports\n  publishes no OpenAPI, so this profile was established by probing the live edge with\n  candidate header names and recording which ones the gateway recognises. Two header\n  names are accepted, corresponding to the provider's two distribution channels\n  (direct subscription and the RapidAPI marketplace); every other credential shape is\n  rejected at the edge before routing.\nmodel: api-key\noauth2: false\nopenid_connect: false\nmutual_tls: false\nschemes:\n  - id: apisports-key\n  \
  \  type: apiKey\n    in: header\n    name: x-apisports-key\n    channel: direct\n    description: >-\n      API key issued from the API-Sports dashboard (dashboard.api-football.com) and\n      used when calling the sport hosts directly, e.g. v3.football.api-sports.io.\n      One key works across every sport API the account is subscribed to.\n    verified: probed\n    evidence:\n      url: https://v3.football.api-sports.io/status\n      request_header: 'x-apisports-key: <placeholder>'\n      http_status: 200\n      body_excerpt: >-\n        {\"get\":\"status\",\"parameters\":[],\"errors\":{\"token\":\"Error/Missing application\n        key. Go to https://www.api-football.com/documentation-v3 to learn how to get\n        your API application key.\"},\"results\":0,...}\n      reading: >-\n        The header name is recognised — the request passes the edge (HTTP 200) and is\n        rejected by the application's own token check, which names the documentation\n        page.\n  - id: rapidapi-key\n\
  \    type: apiKey\n    in: header\n    name: x-rapidapi-key\n    channel: marketplace\n    description: >-\n      RapidAPI marketplace key, used with the companion x-rapidapi-host header when\n      calling through api-football-v1.p.rapidapi.com and the sibling RapidAPI hosts.\n      Billing and quota are managed by RapidAPI rather than by API-Sports.\n    companion_header: x-rapidapi-host\n    verified: probed\n    evidence:\n      url: https://v3.football.api-sports.io/status\n      request_header: 'x-rapidapi-key: <placeholder>'\n      http_status: 200\n      reading: >-\n        Also recognised at the direct host — the edge accepts either key header name\n        and defers to the application token check.\n  - id: rapidapi-gateway\n    type: apiKey\n    in: header\n    name: x-rapidapi-key\n    channel: marketplace\n    host: api-football-v1.p.rapidapi.com\n    verified: probed\n    evidence:\n      url: https://api-football-v1.p.rapidapi.com/v3/status\n      http_status: 401\n   \
  \   body: '{\"message\":\"Invalid API key. Go to https://docs.rapidapi.com/docs/keys for more info.\"}'\n      reading: >-\n        The marketplace gateway returns a conventional HTTP 401 with its own error\n        envelope — a different failure shape from the direct hosts.\nrejected_schemes:\n  - name: X-API-Key\n    http_status: 403\n    note: Not recognised. Edge returns the 4xHe token error before routing.\n  - name: 'Authorization: Bearer'\n    http_status: 403\n    note: >-\n      Not recognised. API-Sports has no bearer-token, OAuth 2.0 or OpenID Connect\n      surface; /.well-known/openid-configuration and\n      /.well-known/oauth-authorization-server both 404 on api-sports.io.\nfindings:\n  - id: two-layer-auth-failure\n    summary: >-\n      Authentication failure has two distinct shapes and an agent must handle both.\n      An unknown or absent credential header fails at the Cloudflare edge with HTTP\n      403 and error code \"4xHe\"; a recognised header carrying a bad key\
  \ fails at the\n      application with HTTP 200 and the failure described only inside\n      errors.token. A client that branches on HTTP status alone will read the second\n      case as success.\n  - id: auth-precedes-routing\n    summary: >-\n      The edge checks credentials before it resolves the route. A request to a\n      nonexistent path with a recognised key header returns the same 200 + token\n      error as a real path, and the response echoes the requested path back in the\n      \"get\" field verbatim. Unauthenticated route discovery is therefore impossible,\n      and the \"get\" echo must not be read as confirmation that an endpoint exists.\n      (Control probe: /bogusendpoint returned get=\"bogusendpoint\".)\n  - id: no-scopes\n    summary: >-\n      There is no scope, permission or role surface. Access is all-or-nothing per key\n      and is bounded by the subscription plan, not by grants — so no scopes/ artifact\n      is applicable to this provider.\ndocs: https://www.api-football.com/documentation-v3\n\
  maintainers:\n  - FN: Kin Lane\n    email: info@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-sports/refs/heads/main/authentication/api-sports-authentication.yml
summary_line: 3 schemes
tags:
- Sports Data
- Live Scores
- Statistics
- Football
- Basketball
- Baseball
- American Football
- Ice Hockey
- Formula 1
- Rugby
- Volleyball
- Handball
- MMA
- Real-Time
- Fixtures
- Standings
- Odds
---
