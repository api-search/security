---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Adgager Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adgager declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Adgager
provider_slug: adgager
scheme_count: 2
schemes:
- evidence: 'An unauthenticated POST of `{me{id}}` returns {"errors":[{"message":"Unauthenticated.","extensions":{"guards":["sanctum"]}}]}. The `guards: ["sanctum"]` extension names Laravel Sanctum, whose HTTP guard reads a personal-access token from the Authorization: Bearer header.'
  format: Bearer <token>
  header: Authorization
  id: sanctum-bearer
  in: header
  observed: '2026-09-07'
  scheme: bearer
  type: http
- applies_to:
  - countries
  - cities
  - districts
  - regions
  - plans
  - languages
  - sectors
  - positions
  - universities
  - faculties
  evidence: 'Reference-data queries answer with data and no credential. Verified anonymously on 2026-09-07: countries (249 rows), cities, plans (8 rows), languages (2 rows).'
  id: none-anonymous
  type: none
slug: adgager-authentication
source_filename: adgager-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: https://api.adgager.com/graphql\ndocs: null\nnote: >-\n  Adgager publishes no developer documentation, so this profile is read from the live GraphQL\n  endpoint itself rather than from an auth page. derive-authentication.py was not usable here\n  because it reads OpenAPI securitySchemes and this provider ships GraphQL, not OpenAPI.\napi: adgager-graphql\nendpoint: https://api.adgager.com/graphql\ntransport: GraphQL over HTTP POST (Laravel Lighthouse)\nschemes:\n- id: sanctum-bearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: Bearer <token>\n  evidence: >-\n    An unauthenticated POST of `{me{id}}` returns\n    {\"errors\":[{\"message\":\"Unauthenticated.\",\"extensions\":{\"guards\":[\"sanctum\"]}}]}.\n    The `guards: [\"sanctum\"]` extension names Laravel Sanctum, whose HTTP guard reads a\n    personal-access token from the Authorization: Bearer header.\n  observed: '2026-09-07'\n- id:\
  \ none-anonymous\n  type: none\n  evidence: >-\n    Reference-data queries answer with data and no credential. Verified anonymously on\n    2026-09-07: countries (249 rows), cities, plans (8 rows), languages (2 rows).\n  applies_to:\n  - countries\n  - cities\n  - districts\n  - regions\n  - plans\n  - languages\n  - sectors\n  - positions\n  - universities\n  - faculties\ncredential_issuance:\n  self_service: false\n  mechanism: >-\n    Tokens are minted by the platform's own login flow, not by a developer key page. The schema\n    exposes login, socialLogin, register, registerWithRefer, passwordResetRequest and checkAuth\n    mutations, and LoginResponse is the token-bearing type. There is no public API-key console,\n    no documented client-credentials flow, and no published developer program.\n  human_entry_point: https://dash.adgager.com/login\noauth2: false\nopenid_connect: false\nmtls: false\napi_keys: false\nscopes:\n  present: false\n  note: >-\n    No OAuth 2.0 flow and no scope\
  \ surface. Authorization is role-based inside the platform - the\n    schema carries managePermission, updateUserRole, PermissionResponse and an impersonate mutation\n    - but no scope vocabulary is exposed to a client, so no scopes/ artifact is written.\ndiscovery:\n  openid_configuration: not served (404 on every host - see well-known/adgager-well-known.yml)\n  oauth_authorization_server: not served (404 on every host)\n  oauth_protected_resource: not served (404 on every host)\nintrospection:\n  graphql_introspection_enabled: true\n  authenticated: false\n  note: >-\n    Full GraphQL introspection is open to anonymous callers. That is what made this profile\n    possible; it is recorded as an observation, not as a recommendation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adgager/refs/heads/main/authentication/adgager-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Market Research
- Consumer Insights
- Survey
- Advertising
- Advertising Effectiveness
- Brand Measurement
- Panel
- GraphQL
- Turkey
---
