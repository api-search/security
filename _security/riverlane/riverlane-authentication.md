---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Riverlane Authentication
name_suffix: Authentication
oauth_flows: []
overview: Riverlane secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Riverlane
provider_slug: riverlane
scheme_count: 1
schemes:
- applies_to:
  - https://deltakit.riverlane.com/proxy/api/graphql
  - https://deltakit.riverlane.com/proxy/api/data/query/{name}
  - https://deltakit.riverlane.com/proxy/api/v2/tasks/add/{task}
  - https://deltakit.riverlane.com/proxy/api/v2/tasks/get/
  - https://deltakit.riverlane.com/proxy/api/v2/tasks/kill/
  description: A single opaque account token. The docs state the secret is a 32-character string; a malformed token returns "Invalid token header. Secret key should be a 32-character string." Tokens are long-lived but regenerable — regenerating invalidates the previous token immediately.
  format: Bearer <token>
  header: Authorization
  in: header
  name: DeltakitToken
  scheme: bearer
  sources:
  - https://github.com/Deltakit/deltakit/blob/main/deltakit-explorer/src/deltakit_explorer/_api/_auth.py
  - https://github.com/Deltakit/deltakit/blob/main/deltakit-explorer/src/deltakit_explorer/_api/_api_v2_client.py
  type: http
slug: riverlane-authentication
source_filename: riverlane-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://github.com/Deltakit/deltakit/blob/main/docs/guide/authentication.md\ndocs: https://github.com/Deltakit/deltakit/blob/main/docs/guide/authentication.md\nnotes: >-\n  Derived by reading Riverlane's own published authentication guide and the open-source client\n  (deltakit-explorer/_api/_auth.py, _api_v2_client.py, _gql_client.py). Riverlane publishes no\n  OpenAPI, so there are no securitySchemes to parse; this profile is the documented contract.\n  There is no OAuth 2.0 / OIDC surface — /.well-known/openid-configuration,\n  /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource all 404, so\n  no scopes/ artifact is emitted.\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\n  openid_connect: false\n  mtls: false\nschemes:\n- name: DeltakitToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <token>'\n\
  \  description: >-\n    A single opaque account token. The docs state the secret is a 32-character string; a malformed\n    token returns \"Invalid token header. Secret key should be a 32-character string.\" Tokens are\n    long-lived but regenerable — regenerating invalidates the previous token immediately.\n  applies_to:\n  - https://deltakit.riverlane.com/proxy/api/graphql\n  - https://deltakit.riverlane.com/proxy/api/data/query/{name}\n  - https://deltakit.riverlane.com/proxy/api/v2/tasks/add/{task}\n  - https://deltakit.riverlane.com/proxy/api/v2/tasks/get/\n  - https://deltakit.riverlane.com/proxy/api/v2/tasks/kill/\n  sources:\n  - https://github.com/Deltakit/deltakit/blob/main/deltakit-explorer/src/deltakit_explorer/_api/_auth.py\n  - https://github.com/Deltakit/deltakit/blob/main/deltakit-explorer/src/deltakit_explorer/_api/_api_v2_client.py\nprovisioning:\n  self_serve: true\n  cost: free\n  token_page: https://deltakit.riverlane.com/dashboard/token\n  requires_account: true\n\
  \  note: >-\n    Riverlane's launch material describes the access token as free. The token page itself requires\n    a Deltakit account login and could not be read anonymously.\nclient_handling:\n  env_var: DELTAKIT_TOKEN\n  persisted_file: true\n  persisted_note: Client.set_token() writes the token to a local .env-style config file by default\n  set_token_validates: true\n  validation_call: >-\n    GET /api/v2/tasks/get/ with an empty request_id (v2) or a content-endpoint probe (v1); a 401\n    with error_code 6000 means the token is bad\n  tls_verification_toggle: DELTAKIT_DISABLE_TLS_CHECK (debug only; disables certificate validation)\nanonymous_access:\n  supported: false\n  evidence:\n  - {url: 'https://deltakit.riverlane.com/proxy/api/graphql', status: 401, body: '{\"message\":\"No authorisation credentials provided\",\"error_code\":6000}'}\n  - {url: 'https://deltakit.riverlane.com/proxy/api/v2/tasks/get/', status: 401, body: '{\"message\":\"No authorisation credentials provided\"\
  ,\"error_code\":6000}'}\n  - {url: 'https://deltakit.riverlane.com/proxy/api/data/query/decode', status: 401, body: '{\"message\":\"No authorisation credentials provided\",\"error_code\":6000}'}\nx-evidence:\n  fetched: '2026-08-05'\n  probes:\n  - {url: 'https://deltakit.riverlane.com/proxy/api/graphql', method: POST, status: 401, content_type: application/json}\n  - {url: 'https://deltakit.riverlane.com/.well-known/openid-configuration', status: 404}\n  - {url: 'https://deltakit.riverlane.com/.well-known/oauth-authorization-server', status: 404}\n  - {url: 'https://deltakit.riverlane.com/.well-known/oauth-protected-resource', status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/riverlane/refs/heads/main/authentication/riverlane-authentication.yml
summary_line: http · 1 scheme
tags:
- quantum-computing
- quantum-error-correction
- decoders
- scientific-computing
- python-sdk
- graphql
- simulation
- research-tools
- open-source
- hpc
---
