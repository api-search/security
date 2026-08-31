---
api_key_in: []
api_specs:
- filename: academy-software-foundation-hosts-api-openapi.yml
  format: yaml
  label: Academy Software Foundation Hosts API
  slug: academy-software-foundation-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/academy-software-foundation/refs/heads/main/openapi/academy-software-foundation-hosts-api-openapi.yml
- filename: academy-software-foundation-jobs-api-openapi.yml
  format: yaml
  label: Academy Software Foundation Jobs API
  slug: academy-software-foundation-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/academy-software-foundation/refs/heads/main/openapi/academy-software-foundation-jobs-api-openapi.yml
- filename: academy-software-foundation-layers-api-openapi.yml
  format: yaml
  label: Academy Software Foundation Layers API
  slug: academy-software-foundation-layers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/academy-software-foundation/refs/heads/main/openapi/academy-software-foundation-layers-api-openapi.yml
- filename: academy-software-foundation-shows-api-openapi.yml
  format: yaml
  label: Academy Software Foundation Shows API
  slug: academy-software-foundation-shows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/academy-software-foundation/refs/heads/main/openapi/academy-software-foundation-shows-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Academy Software Foundation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Academy Software Foundation declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Academy Software Foundation
provider_slug: academy-software-foundation
scheme_count: 1
schemes:
- algorithm: HS256
  api: academy-software-foundation:academy-software-foundation-jobs-api
  applies_to: every gateway endpoint
  bearer_format: JWT
  exceptions:
  - note: The Swagger UI and the OpenAPI definitions it serves (/swagger/specs/<name>.swagger.json) are the only unauthenticated routes. When the documentation routes are disabled or SWAGGER_DIR is absent, /swagger/ falls through to the authenticated handler and returns 401.
    path: /swagger/
  failure_codes:
  - meaning: Missing or invalid Authorization header
    status: 401
  - meaning: Token validation failed or expired
    status: 403
  header: Authorization
  id: bearerAuth
  issued_by: the studio operating the gateway (shared HMAC secret), not by ASWF
  location: header
  required_claims:
  - sub
  - exp
  scheme: bearer
  type: http
  value_prefix: 'Bearer '
slug: academy-software-foundation-authentication
source_filename: academy-software-foundation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://github.com/AcademySoftwareFoundation/OpenCue/blob/master/docs/_docs/reference/rest-api-reference.md\ndocs: https://www.opencue.io/docs/\nnote: >-\n  ASWF hosts no authenticated API of its own. The only authenticated interface any ASWF project\n  ships is the OpenCue REST Gateway, which studios deploy inside their own network; the credential\n  is therefore issued by the deploying studio, not by ASWF. The four OpenAPI documents in this repo\n  were written by API Evangelist from documentation and declare no securityScheme, so this profile\n  is taken from the provider's own REST API reference rather than derived from those specs.\nschemes:\n  - id: bearerAuth\n    api: academy-software-foundation:academy-software-foundation-jobs-api\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    location: header\n    header: Authorization\n    value_prefix: 'Bearer '\n    algorithm: HS256\n    required_claims:\n   \
  \   - sub\n      - exp\n    issued_by: the studio operating the gateway (shared HMAC secret), not by ASWF\n    applies_to: every gateway endpoint\n    exceptions:\n      - path: /swagger/\n        note: >-\n          The Swagger UI and the OpenAPI definitions it serves (/swagger/specs/<name>.swagger.json)\n          are the only unauthenticated routes. When the documentation routes are disabled or\n          SWAGGER_DIR is absent, /swagger/ falls through to the authenticated handler and returns 401.\n    failure_codes:\n      - status: 401\n        meaning: Missing or invalid Authorization header\n      - status: 403\n        meaning: Token validation failed or expired\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_keys: false\nguidance:\n  - Tokens are expected to be short-lived; the reference recommends 1-2 hour expirations.\n  - The reference requires HTTPS in production; the gateway itself speaks plain HTTP by default.\n  - >-\n    There is no ASWF-operated authorization\
  \ server. /.well-known/oauth-authorization-server and\n    /.well-known/openid-configuration were probed on every ASWF host and returned 404 (see\n    well-known/academy-software-foundation-well-known.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/academy-software-foundation/refs/heads/main/authentication/academy-software-foundation-authentication.yml
summary_line: 1 scheme
tags:
- Animation
- Color Management
- Film
- Linux Foundation
- Open-Source
- Rendering
- Standards
- Visual Effects
- VFX
---
