---
anonymous_access: false
api_key_in: []
api_specs:
- filename: brick-brick-server-openapi.yml
  format: yaml
  label: Brick Example Server
  slug: server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brick/refs/heads/main/openapi/brick-brick-server-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Brick Authentication
name_suffix: Authentication
oauth_flows: []
overview: BRICK Schema secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BRICK Schema
provider_slug: brick
scheme_count: 1
schemes:
- applied_to: 12 of 19 operations
  bearerFormat: JWT
  name: HTTPBearer
  note: The only securityScheme in the contract. There are no scopes, so a token that can read a building's telemetry can also actuate its equipment.
  scheme: bearer
  sources:
  - openapi/brick-brick-server-openapi.yml
  type: http
slug: brick-authentication
source_filename: brick-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: derived\nsource: >-\n  openapi/brick-brick-server-openapi.yml (components.securitySchemes + per-operation security) ;\n  https://github.com/BrickSchema/brick-example-server (HTTP 200)\nsummary:\n  types:\n    - http\n  scopes_published: false\n  oauth2_metadata_published: false\nschemes:\n  - name: HTTPBearer\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    sources:\n      - openapi/brick-brick-server-openapi.yml\n    applied_to: 12 of 19 operations\n    note: >-\n      The only securityScheme in the contract. There are no scopes, so a token that can read a\n      building's telemetry can also actuate its equipment.\ntoken_lifecycle:\n  issue:\n    operation: gen_token_brickapi_v1_auth_app_tokens_post\n    path: POST /brickapi/v1/auth/app_tokens\n    parameters:\n      - name: app_name\n        in: query\n        required: false\n        description: The name of an app the user needs to generate a token for\n      - name: token_lifetime\n\
  \        in: query\n        required: false\n        description: Expiration time of the requested token in seconds.\n    returns: 'TokenResponse — token (JWT), name, exp (unix timestamp)'\n  list:\n    operation: get_tokens_brickapi_v1_auth_app_tokens_get\n    path: GET /brickapi/v1/auth/app_tokens\n  revoke:\n    operation: del_token_brickapi_v1_auth_app_tokens__app_token__delete\n    path: DELETE /brickapi/v1/auth/app_tokens/{app_token}\ninteractive_login:\n  flow: google-redirect\n  operations:\n    - get_login_via_google_brickapi_v1_auth_login_get\n    - get_authorize_brickapi_v1_auth_logincallback_get\n    - get_is_registered_brickapi_v1_auth_is_registered_get\n    - post_register_user_brickapi_v1_auth_register_get\n  note: >-\n    /brickapi/v1/auth/login is summarised \"Get Login Via Google\" and /auth/logincallback \"Get\n    Authorize\" — a Google sign-in redirect. Despite that, the contract declares NO oauth2 or\n    openIdConnect securityScheme, publishes no authorization-server\
  \ metadata, and defines no scopes;\n    every /.well-known/openid-configuration and /.well-known/oauth-authorization-server probe on the\n    Brick hosts returned 404 on 2026-09-04. Recorded as http-bearer only.\nunsecured_operations:\n  - get_login_via_google_brickapi_v1_auth_login_get\n  - get_is_registered_brickapi_v1_auth_is_registered_get\n  - get_authorize_brickapi_v1_auth_logincallback_get\ndocs: https://github.com/BrickSchema/brick-example-server\ngap: >-\n  No dedicated authentication documentation page exists — the repository README and the contract are\n  the whole of it. No 401 or 403 response is declared on any secured operation, so an agent cannot\n  tell an auth failure from any other undocumented status.\nmaintainers:\n  - FN: Kin Lane\n    email: info@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brick/refs/heads/main/authentication/brick-authentication.yml
summary_line: http · 1 scheme
tags:
- Building Information Modeling
- BIM
- Smart Buildings
- Ontology
- Semantic Web
- IoT
- HVAC
- Energy Management
---
