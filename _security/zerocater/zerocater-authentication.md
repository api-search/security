---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: probed
name: Zerocater Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zerocater secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zerocater
provider_slug: zerocater
scheme_count: 1
schemes:
- bearer_format: null
  description: Django REST Framework TokenAuthentication. A per-user opaque token is presented on the Authorization header. The server advertises the scheme in its 401 challenge.
  in: header
  name: TokenAuth
  parameter_name: Authorization
  scheme: token
  sources:
  - https://app.zerocater.com/api/v3/user
  - https://github.com/ZeroCater/PyZeroCater/blob/master/zerocater/client.py
  type: http
  value_format: Token <token>
slug: zerocater-authentication
source_filename: zerocater-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: https://app.zerocater.com/api/v3\nsummary:\n  types: [http]\n  scheme: token\n  api_key_in: [header]\n  oauth2_flows: []\n  documented_by_provider: false\nnote: >-\n  Zerocater publishes no authentication documentation and no OpenAPI, so this profile\n  was NOT derived from a specification. It was reconstructed from two real sources:\n  (1) the `WWW-Authenticate: Token` challenge and 401 bodies returned live by\n  app.zerocater.com to anonymous requests, and (2) Zerocater's own open-source Python\n  client, which sets `Authorization: Token <token>` on every request. Nothing here is\n  inferred beyond those two observations.\nschemes:\n- name: TokenAuth\n  type: http\n  scheme: token\n  in: header\n  parameter_name: Authorization\n  value_format: 'Token <token>'\n  bearer_format: null\n  description: >-\n    Django REST Framework TokenAuthentication. A per-user opaque token is presented on\n    the Authorization header. The server\
  \ advertises the scheme in its 401 challenge.\n  sources:\n  - https://app.zerocater.com/api/v3/user\n  - https://github.com/ZeroCater/PyZeroCater/blob/master/zerocater/client.py\ntoken_acquisition:\n  advertised_relation: token_url\n  advertised_url: https://app.zerocater.com/api/v3/login\n  client_behavior: >-\n    PyZeroCater issues an HTTP-Basic-credentialed GET against the token_url relation\n    and reads `token` from the JSON body. It also accepts a pre-issued token directly.\n  observed_status: 404\n  observed_note: >-\n    The advertised login relation returned an HTML 404 to anonymous GET and OPTIONS on\n    2026-08-05, so the current token-issuance route could not be confirmed from the\n    outside. Recorded as observed; not diagnosed and not guessed at.\n  self_service_signup: https://app.zerocater.com/signup\nchallenge_observed:\n  status: 401\n  www_authenticate: Token\n  content_type: application/json\n  body: '{\"detail\":\"Authentication credentials were not provided.\"\
  }'\n  url: https://app.zerocater.com/api/v3/user\nunauthenticated_surface:\n  note: >-\n    A subset of the API answers anonymous requests without a token. Company, meal-list\n    and meal resources return DRF metadata to OPTIONS and return 404 \"Not found.\" —\n    not 401 — to GET with an unknown identifier, which places them outside the\n    token-required set. Stated as an observation of the deployed behavior only.\n  endpoints:\n  - /api/v3\n  - /api/v3/companies/{short_mangled_id}\n  - /api/v3/companies/{short_mangled_id}/meals\n  - /api/v3/meals/{meal_id}\ngaps:\n- No OAuth 2.0, OpenID Connect, mTLS or API-key surface exists.\n- No /.well-known/openid-configuration or /.well-known/oauth-authorization-server (both 404).\n- No published scope, permission or role model, so scopes/ is not applicable.\n- No published key-rotation, token-expiry or revocation policy.\nrelated:\n  discovery: discovery/zerocater-api-v3-discovery.yml\n  errors: errors/zerocater-problem-types.yml\n  conventions:\
  \ conventions/zerocater-conventions.yml\nx-evidence:\n  fetched: '2026-08-05'\n  urls:\n  - url: https://app.zerocater.com/api/v3/user\n    http_status: 401\n  - url: https://app.zerocater.com/api/v3/login\n    http_status: 404\n  - url: https://app.zerocater.com/.well-known/openid-configuration\n    http_status: 404\n  - url: https://app.zerocater.com/.well-known/oauth-authorization-server\n    http_status: 404\n  credentials_used: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zerocater/refs/heads/main/authentication/zerocater-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Food and Beverage
- Catering
- Corporate Services
- Workplace
- Food Delivery
- Hospitality
- Artificial Intelligence
- Ordering
- Marketplace
---
