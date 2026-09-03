---
api_key_in:
- header
- query
api_specs:
- filename: api-league-openapi.json
  format: json
  label: API League Platform
  slug: api-league-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-league/refs/heads/main/openapi/_original/api-league-openapi.json
auth_types:
- apiKey
description: 'API League authenticates with a single API key and nothing else. There is no OAuth, no OIDC, no scopes, no service accounts and no key rotation surface documented — one key grants the whole 55-operation surface, and the plan attached to that key is what varies. Two interchangeable apiKey schemes are declared in the OpenAPI and applied globally, and the provider documents both: `?api-key=YOUR-API-KEY` in the query string, or the `x-api-key` request header.

  The query-string form is the one the provider leads with in its own examples, and it is the weaker of the two — a key in a URL lands in proxy logs, browser history, referrer headers and shell history. An agent should use the x-api-key header. The terms of use place the consequences on the consumer: the key must be kept confidential, must be stripped before posting code to a forum or GitHub, and the account holder is responsible for any charges or harm from a compromised key.'
kind: authentication
layout: security
method: searched
name: Api League Authentication
name_suffix: Authentication
oauth_flows: []
overview: API League secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: API League
provider_slug: api-league
scheme_count: 2
schemes:
- in: query
  name: apiKey
  parameter: api-key
  sources:
  - openapi/api-league-art-openapi.yml
  - openapi/api-league-books-openapi.yml
  - openapi/api-league-food-openapi.yml
  - openapi/api-league-games-openapi.yml
  - openapi/api-league-humor-openapi.yml
  - openapi/api-league-knowledge-openapi.yml
  - openapi/api-league-math-openapi.yml
  - openapi/api-league-media-openapi.yml
  - openapi/api-league-news-openapi.yml
  - openapi/api-league-storage-openapi.yml
  - openapi/api-league-text-openapi.yml
  - openapi/api-league-web-openapi.yml
  type: apiKey
- in: header
  name: headerApiKey
  parameter: x-api-key
  sources:
  - openapi/api-league-art-openapi.yml
  - openapi/api-league-books-openapi.yml
  - openapi/api-league-food-openapi.yml
  - openapi/api-league-games-openapi.yml
  - openapi/api-league-humor-openapi.yml
  - openapi/api-league-knowledge-openapi.yml
  - openapi/api-league-math-openapi.yml
  - openapi/api-league-media-openapi.yml
  - openapi/api-league-news-openapi.yml
  - openapi/api-league-storage-openapi.yml
  - openapi/api-league-text-openapi.yml
  - openapi/api-league-web-openapi.yml
  type: apiKey
slug: api-league-authentication
source_filename: api-league-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: openapi/api-league-art-openapi.yml, openapi/api-league-books-openapi.yml, openapi/api-league-food-openapi.yml,\n  openapi/api-league-games-openapi.yml, openapi/api-league-humor-openapi.yml, openapi/api-league-knowledge-openapi.yml,\n  openapi/api-league-math-openapi.yml, openapi/api-league-media-openapi.yml, openapi/api-league-news-openapi.yml,\n  openapi/api-league-storage-openapi.yml, openapi/api-league-text-openapi.yml, openapi/api-league-web-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api-key\n  sources:\n  - openapi/api-league-art-openapi.yml\n  - openapi/api-league-books-openapi.yml\n  - openapi/api-league-food-openapi.yml\n  - openapi/api-league-games-openapi.yml\n  - openapi/api-league-humor-openapi.yml\n  - openapi/api-league-knowledge-openapi.yml\n  - openapi/api-league-math-openapi.yml\n  - openapi/api-league-media-openapi.yml\n\
  \  - openapi/api-league-news-openapi.yml\n  - openapi/api-league-storage-openapi.yml\n  - openapi/api-league-text-openapi.yml\n  - openapi/api-league-web-openapi.yml\n- name: headerApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/api-league-art-openapi.yml\n  - openapi/api-league-books-openapi.yml\n  - openapi/api-league-food-openapi.yml\n  - openapi/api-league-games-openapi.yml\n  - openapi/api-league-humor-openapi.yml\n  - openapi/api-league-knowledge-openapi.yml\n  - openapi/api-league-math-openapi.yml\n  - openapi/api-league-media-openapi.yml\n  - openapi/api-league-news-openapi.yml\n  - openapi/api-league-storage-openapi.yml\n  - openapi/api-league-text-openapi.yml\n  - openapi/api-league-web-openapi.yml\ndocs: https://apileague.com/docs/authentication/\nprovider: API League\nproviderId: api-league\ndescription: 'API League authenticates with a single API key and nothing else. There is no OAuth, no OIDC,\n  no scopes, no service accounts and no\
  \ key rotation surface documented — one key grants the whole 55-operation\n  surface, and the plan attached to that key is what varies. Two interchangeable apiKey schemes are declared\n  in the OpenAPI and applied globally, and the provider documents both: `?api-key=YOUR-API-KEY` in the\n  query string, or the `x-api-key` request header.\n\n  The query-string form is the one the provider leads with in its own examples, and it is the weaker of\n  the two — a key in a URL lands in proxy logs, browser history, referrer headers and shell history. An\n  agent should use the x-api-key header. The terms of use place the consequences on the consumer: the\n  key must be kept confidential, must be stripped before posting code to a forum or GitHub, and the account\n  holder is responsible for any charges or harm from a compromised key.'\nobtain:\n  signup: https://apileague.com/console/\n  free_tier: true\n  card_required: false\n  note: Keys are issued from the console after a free signup; the Free\
  \ plan needs no payment method.\nexamples:\n- style: query\n  request: GET https://api.apileague.com/search-books?api-key=YOUR-API-KEY&query=romance\n  source: https://apileague.com/docs/authentication/\n- style: header\n  request: 'GET https://api.apileague.com/search-books?query=romance\n\n    x-api-key: YOUR-API-KEY'\n  source: https://apileague.com/docs/authentication/\nfailure:\n  status: 401\n  body: '{\"status\":\"failure\",\"code\":401,\"message\":\"Please read https://apileague.com/docs/authentication\"}'\n  note: Returned for a missing or invalid key AND for every non-existent path on api.apileague.com — a\n    401 on that host is not evidence a path exists.\ngaps:\n- No OAuth 2.0 / OIDC and no scopes — a key is all-or-nothing across all 55 operations.\n- No documented key rotation, expiry, or per-key restriction (IP, referrer, endpoint).\n- The provider's primary documented example puts the secret in the URL query string.\n- No /.well-known/oauth-authorization-server or openid-configuration\
  \ on any host (see well-known/api-league-well-known.yml).\nevidence:\n- url: https://apileague.com/docs/authentication/\n  status: 200\n- url: https://api.apileague.com/\n  status: 401\n- url: https://apileague.com/terms/\n  status: 200\ncross_links:\n  conventions: conventions/api-league-conventions.yml\n  errors: errors/api-league-problem-types.yml\nmaintainers:\n- FN: Kin Lane\n  email: info@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-league/refs/heads/main/authentication/api-league-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- API Marketplace
- Books
- Developer Tools
- Food
- Games
- Humor
- Media
- News
- OpenAPI
- SDK
- Text Processing
- Web Scraping
---
