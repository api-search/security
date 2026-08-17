---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Betalist Authentication
name_suffix: Authentication
oauth_flows: []
overview: BetaList secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BetaList
provider_slug: betalist
scheme_count: 1
schemes:
- description: '"Authenticate all requests with ?access_token=YOUR_TOKEN_HERE". A single opaque bearer-style token passed on the query string; the documentation defines no scopes, no expiry, and no refresh or rotation flow.'
  in: query
  name: access_token
  parameter: access_token
  sources:
  - https://gist.github.com/marckohlbrugge/5a29bf1ba628bb4ca960
  type: apiKey
slug: betalist-authentication
source_filename: betalist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://gist.github.com/marckohlbrugge/5a29bf1ba628bb4ca960\ndocs: https://gist.github.com/marckohlbrugge/5a29bf1ba628bb4ca960\nnote: >-\n  Derived from the BetaList API documentation gist published by founder Marc\n  Kohlbrugge and linked from https://betalist.com/support (\"How do I get access to\n  the BetaList API?\"). BetaList publishes no OpenAPI, so there are no securitySchemes\n  to derive from; every field below is quoted from that documentation or observed on a\n  live unauthenticated request.\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - query\n  oauth2_flows: []\n  self_service: false\n  onboarding: request\nschemes:\n  - name: access_token\n    type: apiKey\n    in: query\n    parameter: access_token\n    description: >-\n      \"Authenticate all requests with ?access_token=YOUR_TOKEN_HERE\". A single opaque\n      bearer-style token passed on the query string; the documentation defines no\n      scopes,\
  \ no expiry, and no refresh or rotation flow.\n    sources:\n      - https://gist.github.com/marckohlbrugge/5a29bf1ba628bb4ca960\ntoken_issuance:\n  self_service: false\n  model: request-and-review\n  channels:\n    - kind: typeform\n      url: https://marc.typeform.com/to/KOdlOu\n      status: 200\n      source: https://gist.github.com/marckohlbrugge/5a29bf1ba628bb4ca960\n      note: '\"Request your API token here\" — the request form named in the API docs.'\n    - kind: contact-form\n      url: https://betalist.com/contact\n      status: 200\n      requires_account: true\n      source: https://betalist.com/support\n      note: >-\n        The support page directs API requests here and asks for (1) intended use of the\n        API, (2) the use case, and (3) estimated request volume; BetaList reviews each\n        request individually. The form itself redirects anonymous visitors to\n        /sign_in, so a BetaList account is required to file the request.\nobserved:\n  - url: https://api.betalist.com/v1/startups\n\
  \    status: 401\n    checked: '2026-08-13'\n    note: >-\n      Unauthenticated request returns 401 with an empty body and no WWW-Authenticate\n      challenge, no error envelope, and no problem+json document.\n  - url: https://api.betalist.com/v1/markets\n    status: 401\n    checked: '2026-08-13'\n  - url: https://api.betalist.com/v1/regions\n    status: 401\n    checked: '2026-08-13'\ngaps:\n  - Token is carried in the query string, so it lands in server logs, browser history and Referer headers; no header-based alternative is documented.\n  - No documented token expiry, rotation, or revocation.\n  - No scopes or permission model — one token grants the whole read surface.\n  - 401 responses carry no body, so a client cannot distinguish a missing token from a revoked one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betalist/refs/heads/main/authentication/betalist-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Startups
- Beta Testing
- Product Discovery
- Early Adopters
- Newsletters
- Startup Directory
- Company Data
- Product Launches
---
