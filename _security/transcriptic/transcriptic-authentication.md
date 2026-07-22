---
api_key_in:
- header
auth_types:
- apiKey
- http
- custom-signature
description: ''
kind: authentication
layout: security
method: searched
name: Transcriptic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Transcriptic secures its APIs with apiKey, http, and custom-signature across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Transcriptic
provider_slug: transcriptic
scheme_count: 4
schemes:
- description: Primary auth. The user's account email and a personal API token (obtained via `transcriptic login` or the web app) are sent on every request as the X-User-Email and X-User-Token headers.
  header_names:
  - X-User-Email
  - X-User-Token
  in: header
  name: UserEmailToken
  source: transcriptic/config.py
  type: apiKey
- description: Alternative browser-session authentication via Cookie, mutually exclusive with token headers.
  in: cookie
  name: SessionCookie
  source: transcriptic/config.py
  type: apiKey
- description: Bearer-token authentication via the Authorization header (StrateosBearerAuth in the official client).
  name: StrateosBearer
  scheme: bearer
  source: transcriptic/config.py
  type: http
- description: RSA signature-based request authentication (StrateosSign in the official client) for signed programmatic access.
  name: StrateosSign
  source: transcriptic/config.py
  type: custom
slug: transcriptic-authentication
source_filename: transcriptic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/strateos/transcriptic/blob/master/transcriptic/config.py\ndocs: https://developers.strateos.com/docs/getting-started-with-the-cli\napi_root: https://secure.strateos.com\nsummary:\n  types: [apiKey, http, custom-signature]\n  api_key_in: [header]\n  notes: >-\n    Token-based auth, no OAuth2 scope surface. The official client authenticates\n    with a per-user email + API token pair sent as request headers; a bearer-token\n    and an RSA request-signing mode are also supported by the client.\nschemes:\n  - name: UserEmailToken\n    type: apiKey\n    in: header\n    header_names:\n      - X-User-Email\n      - X-User-Token\n    description: >-\n      Primary auth. The user's account email and a personal API token (obtained via\n      `transcriptic login` or the web app) are sent on every request as the\n      X-User-Email and X-User-Token headers.\n    source: transcriptic/config.py\n  - name: SessionCookie\n\
  \    type: apiKey\n    in: cookie\n    description: >-\n      Alternative browser-session authentication via Cookie, mutually exclusive with\n      token headers.\n    source: transcriptic/config.py\n  - name: StrateosBearer\n    type: http\n    scheme: bearer\n    description: >-\n      Bearer-token authentication via the Authorization header (StrateosBearerAuth in\n      the official client).\n    source: transcriptic/config.py\n  - name: StrateosSign\n    type: custom\n    description: >-\n      RSA signature-based request authentication (StrateosSign in the official\n      client) for signed programmatic access.\n    source: transcriptic/config.py\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transcriptic/refs/heads/main/authentication/transcriptic-authentication.yml
summary_line: apiKey/http/custom-signature · 4 schemes
tags:
- Company
- Life Sciences
- Laboratory Automation
- Cloud Lab
- Drug Discovery
- Biotechnology
- REST API
- JSON:API
- Autoprotocol
---
