---
api_key_in: []
api_specs:
- filename: usersnap-api-openapi-original.json
  format: json
  label: Usersnap Platform REST API
  slug: usersnap-platform-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usersnap/refs/heads/main/openapi/usersnap-api-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Usersnap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Usersnap secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Usersnap
provider_slug: usersnap
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'The bearer token is a JWT created by you and signed with the JWT secret provided in https://app.usersnap.com/#/settings/rest-api. Start with a default HS256 JWT and add "kid": "<JWT ID>" to the headers, then sign it with the JWT secret and send it as Authorization: Bearer <jwt>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/usersnap-api-openapi-original.json
  type: http
slug: usersnap-authentication
source_filename: usersnap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/usersnap-api-openapi-original.json\ndocs: https://help.usersnap.com/reference/rest-api\nnotes: >-\n  The Usersnap REST API is a gated feature (available on specific plans; enable\n  under Settings > Rest API in app.usersnap.com). Usersnap generates a shared JWT\n  secret plus a JWT ID; the customer self-signs HS256 JWTs (header must include\n  \"kid\": \"<JWT ID>\"; HS512 is explicitly not supported) and sends them as a\n  Bearer token in the Authorization header. The submit and pre-submit endpoints\n  (project api_key in path) also accept unauthenticated calls per the OpenAPI\n  security declaration ({} alternative).\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  bearer_format: JWT\n  jwt:\n    algorithm: HS256\n    header_kid: JWT ID generated in the Usersnap dashboard\n    secret: shared secret generated at https://app.usersnap.com/#/settings/rest-api\n  gated_feature: true\nschemes:\n  - name: bearerAuth\n\
  \    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      The bearer token is a JWT created by you and signed with the JWT secret\n      provided in https://app.usersnap.com/#/settings/rest-api. Start with a\n      default HS256 JWT and add \"kid\": \"<JWT ID>\" to the headers, then sign it\n      with the JWT secret and send it as Authorization: Bearer <jwt>.\n    sources: [openapi/usersnap-api-openapi-original.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usersnap/refs/heads/main/authentication/usersnap-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Feedback
- Bug Tracking
- Customer Experience
- Product Management
- Surveys
- SaaS
---
