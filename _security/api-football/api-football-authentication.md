---
api_key_in: []
auth_types: []
description: API-Football authenticates with a single static API key sent in a request header. There is no OAuth, no OIDC, no bearer/JWT flow and no mTLS. The key is issued from the API-Sports dashboard and the SAME key works across every API-Sports sport surface. Two header names are accepted, and which one you use depends on which of the two distribution channels you bought through.
kind: authentication
layout: security
method: probed
name: Api Football Authentication
name_suffix: Authentication
oauth_flows: []
overview: API Football declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: API Football
provider_slug: api-football
scheme_count: 2
schemes:
- channel: direct
  description: The key issued in the API-Sports dashboard, used when calling the API directly at https://v3.football.api-sports.io. Sent on every request.
  header: x-apisports-key
  host: v3.football.api-sports.io
  id: apisports-key
  in: header
  name: API-Sports direct key
  obtained_at: https://dashboard.api-football.com/register
  rotatable: unknown
  scopes: []
  type: apiKey
- channel: marketplace
  companion_header: x-rapidapi-host
  description: 'The RapidAPI-issued key, used when the subscription was bought through the RapidAPI hub. Requires the companion x-rapidapi-host header naming the RapidAPI edge host. The provider''s own widget library switches base URL on the value of that header: when x-rapidapi-host is not "v3.football.api-sports.io" it calls https://api-football-v1.p.rapidapi.com/v3/ instead.'
  header: x-rapidapi-key
  host: api-football-v1.p.rapidapi.com
  id: rapidapi-key
  in: header
  name: RapidAPI marketplace key
  obtained_at: https://rapidapi.com/api-sports/api/api-football
  scopes: []
  type: apiKey
slug: api-football-authentication
source_filename: api-football-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: API Football\nproviderId: api-football\ngenerated: '2026-09-02'\nmodified: '2026-09-02'\nmethod: probed\nsource: >-\n  Live unauthenticated + bogus-key probes of https://v3.football.api-sports.io/status\n  run 2026-09-02, cross-read against the provider's own widget library at\n  https://widgets.api-sports.io/football/2.0.3/library/standings.js and the\n  documented auth section at\n  https://www.api-football.com/documentation-v3#section/Authentication\ndescription: >-\n  API-Football authenticates with a single static API key sent in a request\n  header. There is no OAuth, no OIDC, no bearer/JWT flow and no mTLS. The key is\n  issued from the API-Sports dashboard and the SAME key works across every\n  API-Sports sport surface. Two header names are accepted, and which one you use\n  depends on which of the two distribution channels you bought through.\nschemes:\n  - id: apisports-key\n    name:\
  \ API-Sports direct key\n    type: apiKey\n    in: header\n    header: x-apisports-key\n    host: v3.football.api-sports.io\n    channel: direct\n    description: >-\n      The key issued in the API-Sports dashboard, used when calling the API\n      directly at https://v3.football.api-sports.io. Sent on every request.\n    obtained_at: https://dashboard.api-football.com/register\n    rotatable: unknown\n    scopes: []\n  - id: rapidapi-key\n    name: RapidAPI marketplace key\n    type: apiKey\n    in: header\n    header: x-rapidapi-key\n    companion_header: x-rapidapi-host\n    host: api-football-v1.p.rapidapi.com\n    channel: marketplace\n    description: >-\n      The RapidAPI-issued key, used when the subscription was bought through the\n      RapidAPI hub. Requires the companion x-rapidapi-host header naming the\n      RapidAPI edge host. The provider's own widget library switches base URL on\n      the value of that header: when x-rapidapi-host is not\n      \"v3.football.api-sports.io\"\
  \ it calls\n      https://api-football-v1.p.rapidapi.com/v3/ instead.\n    obtained_at: https://rapidapi.com/api-sports/api/api-football\n    scopes: []\nevidence:\n  - what: The API host advertises exactly which key headers it accepts.\n    url: https://v3.football.api-sports.io/status\n    http_status: 200\n    header_observed: 'access-control-allow-headers: x-rapidapi-key, x-apisports-key, x-rapidapi-host'\n    fetched: '2026-09-02'\n  - what: >-\n      With NO key header the API returns HTTP 403 and an envelope whose \"get\"\n      field is empty.\n    url: https://v3.football.api-sports.io/status\n    http_status: 403\n    body: >-\n      {\"get\": \"\",\"parameters\": [],\"errors\": {\"token\": \"Missing application key,\n      Check our documentation on how to add your API key in headers.\",\"error\":\n      \"4xHe\"},\"results\": 0,\"paging\": {\"current\": 1,\"total\": 1},\"response\": []}\n    fetched: '2026-09-02'\n  - what: >-\n      With an INVALID key header present the API\
  \ switches to HTTP 200 and a\n      different message. The status code therefore distinguishes \"no credential\n      supplied\" (403) from \"credential supplied but rejected\" (200 + errors.token).\n    url: https://v3.football.api-sports.io/status\n    request_header: 'x-apisports-key: <32-char placeholder>'\n    http_status: 200\n    body: >-\n      {\"get\":\"status\",\"parameters\":[],\"errors\":{\"token\":\"Error/Missing application\n      key. Go to https://www.api-football.com/documentation-v3 to learn how to get\n      your API application\n      key.\"},\"results\":0,\"paging\":{\"current\":1,\"total\":1},\"response\":[]}\n    fetched: '2026-09-02'\n  - what: >-\n      The RapidAPI edge host is a genuinely separate, gated surface (401, not the\n      API-Sports envelope).\n    url: https://api-football-v1.p.rapidapi.com/v3/status\n    http_status: 401\n    fetched: '2026-09-02'\n  - what: The provider's own widget library sets both headers and switches host on them.\n    url:\
  \ https://widgets.api-sports.io/football/2.0.3/library/standings.js\n    http_status: 200\n    fetched: '2026-09-02'\nnotes:\n  - >-\n      AUTH FAILURE IS NOT SIGNALLED BY STATUS CODE ALONE. Once any key header is\n      present, a rejected key still returns HTTP 200 with the failure carried in\n      the body's `errors` object. An agent that branches only on response.ok will\n      read a rejected key as a successful empty result. Always test\n      `errors` and `results` before trusting a 200.\n  - >-\n      No OAuth 2.0 or OpenID Connect surface exists: /.well-known/openid-configuration\n      and /.well-known/oauth-authorization-server return 404 on every host\n      (see well-known/api-football-well-known.yml). There are consequently no\n      scopes to document, and no scopes/ artifact is written.\n  - >-\n      One key spans the whole API-Sports family (football, basketball, baseball,\n      hockey, rugby, volleyball, handball, Formula 1, NFL/AFL). The key is\n      account-scoped,\
  \ not product-scoped.\nmaintainers:\n  - FN: Kin Lane\n    email: info@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-football/refs/heads/main/authentication/api-football-authentication.yml
summary_line: 2 schemes
tags:
- Sports
- Football
- Soccer
- Live Scores
- Statistics
---
