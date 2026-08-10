---
api_key_in:
- header
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Cionic Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CIONIC secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CIONIC
provider_slug: cionic
scheme_count: 3
schemes:
- description: The platform access token sent on every request to the /a, /c and /w services. Researchers obtain it as token.json from the profile menu of the web portal at https://cionic.com/a ("Download Token"); the client reads the "token" key from that file.
  in: header
  name: x-cionic-user
  parameter_name: x-cionic-user
  sources:
  - https://github.com/cionicwear/cionic-data/blob/main/cionic/api.py
  - https://github.com/cionicwear/cionic-data/blob/main/scripts/README.md
  type: apiKey
- description: 'An OAuth access token supplied as Authorization: Bearer and exchanged at GET https://{domain}/oauth/user, whose response carries the platform token in the "atok" field. The client reads it from the CIONIC_ACCESS_TOKEN environment variable when no token file is given.'
  environment_variable: CIONIC_ACCESS_TOKEN
  name: OAuthBearer
  scheme: bearer
  sources:
  - https://github.com/cionicwear/cionic-data/blob/main/cionic/api.py
  token_exchange_endpoint: https://cionic.com/oauth/user
  type: http
- flows:
  - authorizationUrl: https://cionic.com/oauth/authorize
    flow: authorizationCode
    note: No scope reference is published. GET /oauth/authorize 302s to the portal login at /a?redir=%2Foauth%2Fauthorize%3F; GET /oauth/token returns 405, so the token endpoint is POST-only.
    scopes: {}
    tokenUrl: https://cionic.com/oauth/token
  name: OAuth2
  type: oauth2
slug: cionic-authentication
source_filename: cionic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://github.com/cionicwear/cionic-data/blob/main/cionic/api.py\ndocs: https://github.com/cionicwear/cionic-data/blob/main/scripts/README.md\nnote: >-\n  CIONIC publishes no OpenAPI, so no securityScheme could be derived. This profile is\n  read from the first-party open-source client (cionic/api.py, MIT) and confirmed by\n  anonymous probes of the live endpoints. Nothing here required credentials.\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: x-cionic-user\n  type: apiKey\n  in: header\n  parameter_name: x-cionic-user\n  description: >-\n    The platform access token sent on every request to the /a, /c and /w services.\n    Researchers obtain it as token.json from the profile menu of the web portal at\n    https://cionic.com/a (\"Download Token\"); the client reads the \"token\" key from\n    that file.\n  sources:\n  - https://github.com/cionicwear/cionic-data/blob/main/cionic/api.py\n\
  \  - https://github.com/cionicwear/cionic-data/blob/main/scripts/README.md\n- name: OAuthBearer\n  type: http\n  scheme: bearer\n  description: >-\n    An OAuth access token supplied as Authorization: Bearer and exchanged at\n    GET https://{domain}/oauth/user, whose response carries the platform token in\n    the \"atok\" field. The client reads it from the CIONIC_ACCESS_TOKEN environment\n    variable when no token file is given.\n  token_exchange_endpoint: https://cionic.com/oauth/user\n  environment_variable: CIONIC_ACCESS_TOKEN\n  sources:\n  - https://github.com/cionicwear/cionic-data/blob/main/cionic/api.py\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cionic.com/oauth/authorize\n    tokenUrl: https://cionic.com/oauth/token\n    scopes: {}\n    note: >-\n      No scope reference is published. GET /oauth/authorize 302s to the portal login\n      at /a?redir=%2Foauth%2Fauthorize%3F; GET /oauth/token returns 405, so the token\n\
  \      endpoint is POST-only.\nlogin:\n  style: email-magic-link\n  url: https://cionic.com/a\n  description: >-\n    The researcher and clinician portal takes an email address and mails a sign-in\n    link; the portal then exposes a downloadable token and, for mobile, a \"Gateway\"\n    token authorisation flow through the CIONIC app.\nauthorization_model:\n  scope: per-organization roles\n  roles:\n  - name: analyst\n    id: 1\n  - name: collector\n    id: 2\n  - name: admin\n    id: 3\n  grant_endpoint: POST /a/v{version}/{org}/accounts/{xid}/roles\n  revoke_endpoint: DELETE /a/v{version}/{org}/accounts/{xid}/roles/{role_id}\n  note: Role administration requires the org admin role.\nx-evidence:\n- url: https://cionic.com/a/v2.0/accounts/@me\n  http_status: 401\n  content_type: application/json\n  body: '{\"error\":\"Unauthorized\"}'\n  fetched: '2026-08-09'\n- url: https://cionic.com/oauth/authorize\n  http_status: 302\n  location: /a?redir=%2Foauth%2Fauthorize%3F\n  fetched: '2026-08-09'\n\
  - url: https://cionic.com/oauth/token\n  http_status: 405\n  note: GET rejected; token endpoint is POST-only\n  fetched: '2026-08-09'\n- url: https://raw.githubusercontent.com/cionicwear/cionic-data/main/cionic/api.py\n  http_status: 200\n  fetched: '2026-08-09'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cionic/refs/heads/main/authentication/cionic-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Health
- Medical Devices
- Wearables
- Neurotechnology
- Research
- Clinical Research
- Biomechanics
- Rehabilitation
- Digital Health
---
