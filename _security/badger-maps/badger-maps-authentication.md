---
api_key_in:
- header
api_specs:
- filename: badger-maps-accounts-api-openapi.yml
  format: yaml
  label: Badger Maps Accounts API
  slug: badger-maps-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/openapi/badger-maps-accounts-api-openapi.yml
- filename: badger-maps-check-ins-api-openapi.yml
  format: yaml
  label: Badger Maps Check-Ins API
  slug: badger-maps-check-ins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/openapi/badger-maps-check-ins-api-openapi.yml
- filename: badger-maps-locations-api-openapi.yml
  format: yaml
  label: Badger Maps Locations API
  slug: badger-maps-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/openapi/badger-maps-locations-api-openapi.yml
- filename: badger-maps-routes-api-openapi.yml
  format: yaml
  label: Badger Maps Routes API
  slug: badger-maps-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/openapi/badger-maps-routes-api-openapi.yml
- filename: badger-maps-users-api-openapi.yml
  format: yaml
  label: Badger Maps Users API
  slug: badger-maps-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/openapi/badger-maps-users-api-openapi.yml
auth_types:
- apiKey
description: Badger Maps API v2 uses a single static token sent in an Authorization header with the non-standard scheme word "Token" (not "Bearer"). There is no OAuth, no OIDC, no mTLS, no signed requests and no scope model - one key carries the full permission set of the user it belongs to. Upgraded from derived to searched on 2026-08-13 against the provider's own published API Blueprint, which documents both the header format and the credential-issuing endpoint.
kind: authentication
layout: security
method: searched
name: Badger Maps Authentication
name_suffix: Authentication
oauth_flows: []
overview: Badger Maps secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Badger Maps
provider_slug: badger-maps
scheme_count: 1
schemes:
- description: 'Token authentication. Every request carries "Authorization: Token <api_key>". The scheme word is literally "Token" - an RFC 6750 "Bearer" prefix will not authenticate.'
  example_placeholder: abcdefg12345678
  format: 'Authorization: Token <api_key>'
  in: header
  name: tokenAuth
  parameter: Authorization
  scheme_word: Token
  sources:
  - openapi/_original/badger-maps-openapi.yml
  - openapi/_original/badger-maps-apiary-blueprint.apib
  type: apiKey
slug: badger-maps-authentication
source_filename: badger-maps-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://jsapi.apiary.io/apis/badgerupdatedapi.apib\ndocs: https://badgerupdatedapi.docs.apiary.io/#introduction/authorization\nprovider: Badger Maps\nproviderId: badger-maps\ndescription: >-\n  Badger Maps API v2 uses a single static token sent in an Authorization header\n  with the non-standard scheme word \"Token\" (not \"Bearer\"). There is no OAuth,\n  no OIDC, no mTLS, no signed requests and no scope model - one key carries the\n  full permission set of the user it belongs to. Upgraded from derived to\n  searched on 2026-08-13 against the provider's own published API Blueprint,\n  which documents both the header format and the credential-issuing endpoint.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  scopes: none\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  scheme_word: Token\n  format: 'Authorization: Token <api_key>'\n  example_placeholder:\
  \ abcdefg12345678\n  description: >-\n    Token authentication. Every request carries \"Authorization: Token <api_key>\".\n    The scheme word is literally \"Token\" - an RFC 6750 \"Bearer\" prefix will not\n    authenticate.\n  sources:\n  - openapi/_original/badger-maps-openapi.yml\n  - openapi/_original/badger-maps-apiary-blueprint.apib\ncredential_issuance:\n  self_serve: false\n  gate: >-\n    API/Developer Key access is included with paid plans but must be switched on\n    per team by Badger Maps support. Email support@badgermapping.com to have the\n    key enabled. Until it is enabled the key returns 401 exactly as a bad key\n    does, which makes the gate hard to diagnose from responses alone.\n  contact: support@badgermapping.com\n  runtime_exchange:\n    operation: openapi/badger-maps-users-api-openapi.yml#login\n    path: POST /login/\n    request_encoding: application/x-www-form-urlencoded\n    request_fields: [username, password]\n    response_fields: [token, status, user_id]\n\
  \    note: >-\n      Returns HTTP 200 on failure as well as success; the outcome is in the\n      \"status\" string. See errors/badger-maps-error-codes.yml for the full status\n      vocabulary.\nauthorization_model:\n  scopes: false\n  roles:\n    manager: >-\n      Profile carries is_manager. A manager token may list a managed user's\n      accounts by passing the rn query parameter to GET /customers/, and may\n      reassign an account by sending account_owner on PATCH /customers/{id}/.\n  per_key_permissions: false\n  note: >-\n    No scope, audience or permission surface. Authorization is entirely a\n    property of the user the token belongs to.\nrotation_and_revocation:\n  documented: false\n  note: >-\n    No key rotation, expiry, or revocation procedure is published, and no\n    endpoint lists or revokes issued keys.\ntransport:\n  https_required: true\n  tls_version_observed: TLSv1.3\n  hsts: true\n  source: security/badger-maps-domain-security.yml\ngaps:\n- No OAuth 2.0 or OpenID\
  \ Connect; /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server both 404 on every host.\n- No scopes, so a key cannot be least-privileged for an agent or an integration.\n- No documented key rotation, expiry or revocation.\n- Non-standard \"Token\" scheme word rather than RFC 6750 \"Bearer\".\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/authentication/badger-maps-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Field Sales
- Route Planning
- Mapping
- CRM
- Sales Enablement
- Territory Management
---
