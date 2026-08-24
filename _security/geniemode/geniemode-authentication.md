---
api_key_in: []
api_specs:
- filename: geniemode-cataloguing-api-swagger-2.0.json
  format: json
  label: Geniemode Cataloguing API
  slug: geniemode-cataloguing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geniemode/refs/heads/main/openapi/geniemode-cataloguing-api-swagger-2.0.json
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Geniemode Authentication
name_suffix: Authentication
oauth_flows: []
overview: Geniemode declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Geniemode
provider_slug: geniemode
scheme_count: 1
schemes:
- bearer_format: JWT
  confidence: medium
  declared_in_spec: false
  evidence: GET /api/auth/login (operationId loginUsingGET) returns AuthorisationResponsePayload, whose properties are access_token, refresh_token, token, user_id, user_name and roles[] - the shape of a JWT access/refresh pair with role claims. No securityScheme is declared for it.
  id: bearer-jwt
  scheme: bearer
  type: http
slug: geniemode-authentication
source_filename: geniemode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-21'\nmethod: derived\nsource: openapi/geniemode-cataloguing-api-swagger-2.0.json + live 401 probes of https://portal.geniemode.com/api/*\nnote: >-\n  The Swagger 2.0 document declares NO securityDefinitions block and no operation carries a\n  security requirement, so the machine-readable contract does not describe how to authenticate.\n  The auth model below is derived from the authorisation operations the spec DOES declare plus the\n  live, unauthenticated response behaviour observed on 2026-08-21. Geniemode publishes no public\n  authentication documentation.\nspec_declares_security: false\nschemes:\n- id: bearer-jwt\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  declared_in_spec: false\n  confidence: medium\n  evidence: >-\n    GET /api/auth/login (operationId loginUsingGET) returns AuthorisationResponsePayload, whose\n    properties are access_token, refresh_token, token, user_id, user_name and roles[] - the shape of\n    a JWT access/refresh\
  \ pair with role claims. No securityScheme is declared for it.\nflows:\n- name: password-login\n  operation_id: loginUsingGET\n  method: GET\n  path: /api/auth/login\n  parameters:\n  - name: encodedAuthString\n    in: query\n    required: false\n    type: string\n    note: >-\n      Credentials are passed as a single encoded string in the QUERY STRING of a GET request.\n      Query strings are logged by proxies, browsers and server access logs; a credential-bearing\n      GET is a materially weaker pattern than a POST body and is recorded here as an observation of\n      the published contract, not a recommendation.\n  returns: AuthorisationResponsePayload\n- name: forgot-password\n  operation_id: forgotPasswordUsingGET\n  path: /api/auth/ForgotPassword\n- name: reset-password\n  operation_id: resetPasswordUsingGET\n  path: /api/auth/ResetPassword\nauthorization:\n  model: role-based\n  evidence: AuthorisationResponsePayload.roles is an array of role strings.\n  scopes_published: false\n\
  \  note: >-\n    No OAuth 2.0 or OpenID Connect surface was found. /.well-known/openid-configuration and\n    /.well-known/oauth-authorization-server return the portal SPA shell, not a discovery document.\n    There is therefore no scopes/ artifact - this is a key/session provider, not an OAuth provider.\nobserved_behaviour:\n- probe: https://portal.geniemode.com/api/\n  status: 401\n  body: '{\"timestamp\":...,\"status\":401,\"error\":\"Unauthorized\",\"path\":\"/api/\"}'\n- probe: https://portal.geniemode.com/api/v1/orders\n  status: 401\n- probe: https://portal.geniemode.com/api/v1/skus/elastic-search\n  status: 401\npublic_access: none\npublic_access_note: >-\n  Every operation in the contract requires an authenticated portal session. Geniemode operates no\n  self-service developer signup for the API; portal accounts are provisioned to buyers, suppliers,\n  sales agents and internal staff.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geniemode/refs/heads/main/authentication/geniemode-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Sourcing
- Supply Chain
- Procurement
- B2B Commerce
- Manufacturing
- Logistics
- Textiles
- Apparel
- Furniture
- Quality Control
- India
---
