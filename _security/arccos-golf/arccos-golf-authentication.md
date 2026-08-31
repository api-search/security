---
api_key_in: []
api_specs:
- filename: arccos-golf-clubs-api-openapi.yml
  format: yaml
  label: Arccos Golf Clubs API
  slug: arccos-golf-clubs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arccos-golf/refs/heads/main/openapi/arccos-golf-clubs-api-openapi.yml
- filename: arccos-golf-courses-api-openapi.yml
  format: yaml
  label: Arccos Golf Courses API
  slug: arccos-golf-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arccos-golf/refs/heads/main/openapi/arccos-golf-courses-api-openapi.yml
- filename: arccos-golf-rounds-api-openapi.yml
  format: yaml
  label: Arccos Golf Rounds API
  slug: arccos-golf-rounds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arccos-golf/refs/heads/main/openapi/arccos-golf-rounds-api-openapi.yml
- filename: arccos-golf-users-api-openapi.yml
  format: yaml
  label: Arccos Golf Users API
  slug: arccos-golf-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arccos-golf/refs/heads/main/openapi/arccos-golf-users-api-openapi.yml
- filename: arccos-golf-webhooks-api-openapi.yml
  format: yaml
  label: Arccos Golf Webhooks API
  slug: arccos-golf-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arccos-golf/refs/heads/main/openapi/arccos-golf-webhooks-api-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Arccos Golf Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Arccos Golf secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Arccos Golf
provider_slug: arccos-golf
scheme_count: 2
schemes:
- applies_to: users, rounds, round stats and clubs operations
  flows:
  - authorizationUrl: https://signin.arccosgolf.com/login
    client_authentication: client_id (+ client_secret when issued)
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    redirectUrl: https://api.arccosgolf.com/oauth2-redirect.html
    revocationUrl: https://api.arccosgolf.com/oauth2/revoke
    scopes: 4
    tokenUrl: https://api.arccosgolf.com/oauth2/token
    token_request_encoding: application/x-www-form-urlencoded
  name: AccessCodeAuth
  sources:
  - openapi/arccos-golf-on-course-data-api-openapi.yml
  - https://api.arccosgolf.com/swagger.json
  type: oauth2
- applies_to: the /v5/webhooks registration operations (GET, POST, DELETE)
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/arccos-golf-on-course-data-api-openapi.yml
  type: http
slug: arccos-golf-authentication
source_filename: arccos-golf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: >-\n  https://api.arccosgolf.com/swagger.json (info.description — published Authentication section) +\n  openapi/arccos-golf-on-course-data-api-openapi.yml securityDefinitions\ndocs: https://api.arccosgolf.com/swagger\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - authorizationCode\n  access_model: >-\n    Access to the On-Course Data API is restricted. Arccos issues a client id and (optionally) a client secret to\n    approved third parties; the ability to request each scope on behalf of a user is granted per client by Arccos.\n    Client registration is not self-serve — the published contact is john@arccosgolf.com.\n  anonymous_operations:\n  - handle_search_courses.get./v5/courses\n  - handle_get_one_course.get./v5/courses/{courseId}\n  - handle_get_one_course_version.get./v5/courses/{courseId}/versions/{courseVersion}\n  anonymous_note: >-\n    The three course-catalog operations declare no security requirement\
  \ in the spec, and a probe on 2026-08-06\n    confirmed GET https://api.arccosgolf.com/v5/courses?name=Pebble&limit=2 returns 200 with real course data and\n    no Authorization header. Every other path returns 401 {\"error\":{\"code\":40101,...}} with\n    WWW-Authenticate: Bearer realm=\"arccos\".\nschemes:\n- name: AccessCodeAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://signin.arccosgolf.com/login\n    tokenUrl: https://api.arccosgolf.com/oauth2/token\n    revocationUrl: https://api.arccosgolf.com/oauth2/revoke\n    redirectUrl: https://api.arccosgolf.com/oauth2-redirect.html\n    scopes: 4\n    grant_types:\n    - authorization_code\n    - refresh_token\n    token_request_encoding: application/x-www-form-urlencoded\n    client_authentication: client_id (+ client_secret when issued)\n  applies_to: users, rounds, round stats and clubs operations\n  sources:\n  - openapi/arccos-golf-on-course-data-api-openapi.yml\n  - https://api.arccosgolf.com/swagger.json\n\
  - name: BasicAuth\n  type: http\n  scheme: basic\n  applies_to: the /v5/webhooks registration operations (GET, POST, DELETE)\n  sources:\n  - openapi/arccos-golf-on-course-data-api-openapi.yml\ntokens:\n- name: id_token\n  purpose: >-\n    Returned only when the openid scope is requested. Carries basic user information; explicitly documented as NOT\n    usable to authenticate requests. Its custom:arccosUserId claim supplies the {userId} path parameter used by\n    almost every operation.\n  usable_for_requests: false\n- name: access_token\n  purpose: 'Bearer token presented as `Authorization: Bearer {access_token}` on authenticated requests.'\n  usable_for_requests: true\n  lifetime: short-lived; the published docs leave the exact TTL as \"X hours\"\n- name: refresh_token\n  purpose: >-\n    Exchanged at the token endpoint (grant_type=refresh_token) for a fresh token set; revocable at\n    /oauth2/revoke either by token or by arccos_user_id.\n  usable_for_requests: false\n  lifetime: the\
  \ published docs leave the exact TTL as \"X days\"\nnotes:\n- Scopes cannot be added retroactively — a user must re-authorize the client for any scope not requested initially.\n- The openid scope is mandatory for every operation whose path contains {userId}.\n- >-\n  The identity provider behind signin.arccosgolf.com is an Amazon Cognito hosted UI (the webhook\n  accountDisconnected payload names its client identifier a \"cognito-client-id\"); a bare GET of\n  https://signin.arccosgolf.com/login returns 400 without client_id/response_type parameters.\nstorefront_authentication:\n  note: >-\n    Separate and unrelated to the golf-data API. The Shopify storefront at www.arccosgolf.com publishes an\n    OpenID Connect discovery document delegating customer-account auth to Shopify.\n  issuer: https://shopify.com/authentication/7805525\n  discovery: well-known/arccos-golf-openid-configuration.json\n  scopes_supported:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n\
  cross_links:\n  scopes: scopes/arccos-golf-scopes.yml\n  conventions: conventions/arccos-golf-conventions.yml\n  errors: errors/arccos-golf-problem-types.yml\n  well_known: well-known/arccos-golf-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arccos-golf/refs/heads/main/authentication/arccos-golf-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- golf
- sports-technology
- wearables
- iot
- shot-tracking
- sports-analytics
- performance-analytics
- geospatial
- consumer-hardware
- Webhook
- Authentication
- MCP
- E-Commerce
---
