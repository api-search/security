---
api_key_in: []
api_specs:
- filename: thoughtspot-rest-v2-openapi-original.json
  format: json
  label: ThoughtSpot Public REST API v2.0
  slug: thoughtspot-public-rest-api-v20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thoughtspot/refs/heads/main/openapi/thoughtspot-rest-v2-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Thoughtspot Authentication
name_suffix: Authentication
oauth_flows: []
overview: ThoughtSpot secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ThoughtSpot
provider_slug: thoughtspot
scheme_count: 1
schemes:
- format: Bearer <access_token>
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/thoughtspot-rest-v2-openapi-original.json
  type: http
slug: thoughtspot-authentication
source_filename: thoughtspot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/thoughtspot-rest-v2-openapi-original.json\ndocs: https://developers.thoughtspot.com/docs/api-authv2\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  token_endpoints:\n  - POST /api/rest/2.0/auth/token/full\n  - POST /api/rest/2.0/auth/token/object\n  - GET /api/rest/2.0/auth/session/token\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <access_token>'\n  sources:\n  - openapi/thoughtspot-rest-v2-openapi-original.json\nnotes:\n  overview: >-\n    The ThoughtSpot Public REST API v2.0 uses bearer-token authentication. All\n    191 operations require an Authorization header carrying an access token\n    (global security requirement bearerAuth on every operation).\n  obtaining_tokens:\n  - >-\n    Full access token — POST /api/rest/2.0/auth/token/full with username +\n    password (or secret_key for trusted auth) returns a bearer token with\
  \ the\n    caller's full privileges. operationId getFullAccessToken.\n  - >-\n    Object/scoped access token — POST /api/rest/2.0/auth/token/object issues a\n    token scoped to specific metadata objects for embed use cases. operationId\n    getObjectAccessToken.\n  - >-\n    Current user token — GET /api/rest/2.0/auth/session/token returns a token\n    for the currently logged-in session. operationId getCurrentUserToken.\n  login_sso:\n  - Trusted authentication (secret_key based) for embedded deployments.\n  - SAML 2.0 and OpenID Connect (OIDC) for interactive user login (SSO).\n  session:\n  - >-\n    Session-based login (POST /api/rest/2.0/auth/session/login) and logout\n    (POST /api/rest/2.0/auth/session/logout) are also supported alongside\n    token auth.\ndocs_pages:\n- https://developers.thoughtspot.com/docs/api-authv2\n- https://developers.thoughtspot.com/docs/api-auth-session\n- https://developers.thoughtspot.com/docs/rest-api-getstarted\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thoughtspot/refs/heads/main/authentication/thoughtspot-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Enterprise Software
- Analytics
- Business Intelligence
- Data
- Embedded Analytics
- Artificial Intelligence
- Agents
- REST API
---
