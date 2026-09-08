---
anonymous_access: false
api_key_in: []
api_specs:
- filename: adonmoprivatelimited-adonmo-api.json
  format: json
  label: Adonmo API
  slug: adonmoprivatelimited-adonmo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adonmoprivatelimited/refs/heads/main/openapi/adonmoprivatelimited-adonmo-api.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Adonmoprivatelimited Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adonmo Private Limited declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Adonmo Private Limited
provider_slug: adonmoprivatelimited
scheme_count: 1
schemes:
- description: A bearer access token supplied in the standard HTTP Authorization header. Adonmo names the credential "access_token" in its error envelope. Not declared in the OpenAPI document; inferred from live response behaviour.
  evidence:
    bad_credential:
      body: HTML "401 Unauthorized" (Werkzeug/Flask default error page)
      request: 'GET https://api.adonmo.com/ops_portal/api/spots?page=1&page_size=1 with header Authorization: Bearer <invalid>'
      status: 401
    no_credential:
      body: '{"errors":["access_token is required."]}'
      request: GET https://api.adonmo.com/ops_portal/api/spots?page=1&page_size=1
      status: 400
  id: bearer_access_token
  in: header
  method: probed
  name: Authorization
  scheme: bearer
  type: http
slug: adonmoprivatelimited-authentication
source_filename: adonmoprivatelimited-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: 'openapi/adonmoprivatelimited-adonmo-api.json (which declares no securitySchemes)\n  plus live unauthenticated probes of https://api.adonmo.com/ops_portal/api/spots and\n  /ops_portal/api/spot/{uuid} on 2026-09-07'\napi: Adonmo API\nsummary: 'The published OpenAPI document declares NO components.securitySchemes and NO\n  security requirement on either operation, so the contract itself is silent on\n  authentication. The live API is not: every operation is protected, and the mechanism\n  was established by probing rather than read from the spec. This is a real contract gap\n  — an agent reading only the spec would conclude the API is anonymous.'\nspec_declares_auth: false\nschemes:\n- id: bearer_access_token\n  type: http\n  scheme: bearer\n  in: header\n  name: Authorization\n  method: probed\n  description: 'A bearer access token supplied in the standard HTTP Authorization header.\n    Adonmo names the credential \"access_token\"\
  \ in its error envelope. Not declared in the\n    OpenAPI document; inferred from live response behaviour.'\n  evidence:\n    no_credential:\n      request: 'GET https://api.adonmo.com/ops_portal/api/spots?page=1&page_size=1'\n      status: 400\n      body: '{\"errors\":[\"access_token is required.\"]}'\n    bad_credential:\n      request: 'GET https://api.adonmo.com/ops_portal/api/spots?page=1&page_size=1 with\n        header Authorization: Bearer <invalid>'\n      status: 401\n      body: 'HTML \"401 Unauthorized\" (Werkzeug/Flask default error page)'\nplacements_ruled_out:\n  note: 'Each of these was probed and still returned the 400 \"access_token is required\"\n    envelope, so none of them is the credential channel.'\n  placements:\n  - placement: query parameter access_token\n    status: 400\n  - placement: request header access_token\n    status: 400\n  - placement: request header X-Access-Token\n    status: 400\n  - placement: cookie access_token\n    status: 400\noauth2: false\n\
  oauth_scopes: false\nscopes_artifact: 'not applicable — no oauth2 securityScheme is declared and no OAuth\n  documentation was found, so scopes/ is deliberately absent rather than empty'\nmtls: false\nopenid_connect: false\ntoken_acquisition:\n  documented: false\n  note: 'No public documentation was found describing how a developer obtains an access\n    token. There is no developer signup, no key-issuance page, and no self-service\n    credential surface on any Adonmo host. The Swagger UI at https://api.adonmo.com/apidocs/\n    renders with auth_config unset, so it offers no Authorize control either. Access\n    appears to be provisioned internally or to contracted partners.'\nerror_envelope:\n  shape: '{\"errors\": [\"<message>\", ...]}'\n  content_type: application/json\n  note: 'A non-RFC-9457 array-of-strings envelope. See errors/adonmoprivatelimited-problem-types.yml.'\ndocs: https://api.adonmo.com/apidocs/\ngaps:\n- 'securitySchemes are absent from the OpenAPI document even though\
  \ the API enforces\n  authentication on every operation.'\n- 'No documented token-acquisition flow, so an integrator cannot self-serve.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adonmoprivatelimited/refs/heads/main/authentication/adonmoprivatelimited-authentication.yml
summary_line: 1 scheme
tags:
- Advertising
- Digital Out-of-Home
- DOOH
- Digital Signage
- AdTech
- Content Management
- Marketing
- India
- Company
---
