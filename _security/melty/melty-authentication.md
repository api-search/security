---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Melty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Melty declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Melty
provider_slug: melty
scheme_count: 0
schemes: []
slug: melty-authentication
source_filename: melty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: >-\n  https://github.com/meltygroup/kisee (README), https://github.com/meltygroup/pasee (docs/API.rst),\n  https://kisee.readthedocs.io/en/latest/, https://pasee.readthedocs.io/en/latest/\ndocs: https://kisee.readthedocs.io/en/latest/\nnote: >-\n  Written from the published documentation of the two open-source servers, not derived from an\n  OpenAPI — none exists (derive-authentication.py found 0 auth profiles for this provider). Melty\n  itself exposes no authenticated API, so there is no Melty-issued credential of any kind: nothing\n  below is obtained from Melty, it is what the software you host does once you run it.\napis:\n- aid: melty-kisee\n  schemes:\n  - id: password-grant\n    type: http\n    scheme: basic-equivalent\n    location: request body\n    endpoint: POST /jwt/\n    description: >-\n      Unauthenticated POST of `{\"username\": \"...\", \"password\": \"...\"}` to `/jwt/` returns a CoreJSON\n      document\
  \ containing a `tokens[]` array of JWTs. This is the only credential exchange Kisee\n      performs.\n  - id: bearer-jwt\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    algorithm: ES256\n    description: >-\n      Issued JWTs carry `iss`, `sub`, `exp` and `jti` claims and are signed with an EC key pair using\n      ES256. The signing key and issuer are set by the operator in the server's settings file.\n  self_registration:\n    supported: true\n    endpoint: POST /users/\n    description: >-\n      A new user may self-register by POSTing `{\"username\", \"password\", \"email\"}` to `/users/`;\n      the server answers 201 Created with a `Location` header. Whether this is enabled is an\n      operator decision.\n  identity_backends:\n    pluggable: true\n    documented: [in-memory demo backend, PostgreSQL, LDAP, flat file, any custom Python class]\n    note: The operator supplies the backend; Kisee ships a demo backend and a PostgreSQL schema.\n- aid: melty-pasee\n  schemes:\n\
  \  - id: bearer-jwt\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    algorithm: ES256\n    description: >-\n      Pasee validates and issues ES256-signed JWTs and layers group membership on top. Tokens are\n      managed through the `tokens` resource advertised in the JSON-Home document at `/`.\n  federation:\n    supported: true\n    providers_documented: [one or many Kisee instances, Twitter, GitHub]\n    note: >-\n      Pasee is a layer over multiple identity managers; the specific external providers enabled are\n      an operator configuration choice, not a Melty-hosted service.\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_keys: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/melty/refs/heads/main/authentication/melty-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Consumer
- Media
- Publishing
- News
- Entertainment
- France
- Advertising
- Open Source
- Identity
---
