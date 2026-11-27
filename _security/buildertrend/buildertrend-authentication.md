---
anonymous_access: false
api_key_in: []
api_specs:
- filename: buildertrend-authentication-api-openapi.yml
  format: yaml
  label: Buildertrend Authentication API
  slug: buildertrend-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildertrend/openapi/buildertrend-authentication-api-openapi.yml
- filename: buildertrend-jobs-api-openapi.yml
  format: yaml
  label: Buildertrend Jobs API
  slug: buildertrend-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildertrend/openapi/buildertrend-jobs-api-openapi.yml
- filename: buildertrend-tasks-api-openapi.yml
  format: yaml
  label: Buildertrend Tasks API
  slug: buildertrend-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildertrend/openapi/buildertrend-tasks-api-openapi.yml
- filename: buildertrend-utility-api-openapi.yml
  format: yaml
  label: Buildertrend Utility API
  slug: buildertrend-utility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildertrend/openapi/buildertrend-utility-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Buildertrend Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode (PKCE, documented in prose; not declared as a securityScheme)
overview: Buildertrend secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode (PKCE, documented in prose; not declared as a securityScheme) flow(s).
provider_name: Buildertrend
provider_slug: buildertrend
scheme_count: 3
schemes:
- description: 'Exchange your app''s consumer key and secret at `POST /token`, then send the returned token as `Authorization: Bearer <token>`.'
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /api/token
  name: clientCredentials
  prerequisites:
  - An app created in the developer portal (My apps), which issues a consumer key (OAuth client ID) and consumer secret (client secret).
  - A linked Buildertrend account; until linked, calls return 401 api_key_not_linked.
  sources:
  - openapi/buildertrend-openapi.yml
  - https://developer.buildertrend.com/get-started
  token_lifetime: Tokens last 30 minutes. There's no refresh token; request a new one when it expires.
  type: oauth2
- description: Consumer key as the username, consumer secret as the password (used at POST /api/token). The key and secret may instead be sent as client_id and client_secret form fields.
  name: consumerCredentials
  scheme: basic
  sources:
  - openapi/buildertrend-openapi.yml
  type: http
- declared_in_spec: false
  description: A standard OAuth 2.0 authorization code grant with PKCE (RFC 7636), against Buildertrend's sign-in service rather than this API. Documented in the OpenAPI info.description, not as a securityScheme. The signing-in user's account needs Open API access.
  flows:
  - audience: https://openapi.buildertrend.net/
    authorizationUrl: https://login.buildertrend.com/authorize
    flow: authorizationCode
    pkce: S256 (RFC 7636)
    public_client: true
    redirect_uri: http://localhost:8484
    scopes:
    - openid
    - profile
    - email
    - offline_access
    tokenUrl: https://login.buildertrend.com/oauth/token
  name: userSignInPkce
  sources:
  - openapi/buildertrend-openapi.yml
  token_lifetime: access token valid for 24 hours; refresh tokens rotate and last 30 days, or 15 days without use, whichever comes first.
  type: oauth2
slug: buildertrend-authentication
source_filename: buildertrend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: searched\nsource:\n- https://developer.buildertrend.com/get-started\n- https://developer.buildertrend.com/apis/open-api\n- openapi/buildertrend-openapi.yml\ndocs: https://developer.buildertrend.com/get-started\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode (PKCE, documented in prose; not declared as a securityScheme)\n  token_transport: 'Authorization: Bearer <token>'\n  unauthenticated_operations:\n  - hello\nschemes:\n- name: clientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /api/token\n    scopes: 0\n  token_lifetime: Tokens last 30 minutes. There's no refresh token; request a new one when it expires.\n  description: 'Exchange your app''s consumer key and secret at `POST /token`, then send the\n    returned token as `Authorization: Bearer <token>`.'\n  prerequisites:\n  - An app created in the developer portal (My apps), which issues a consumer\
  \ key (OAuth client ID) and consumer secret (client secret).\n  - A linked Buildertrend account; until linked, calls return 401 api_key_not_linked.\n  sources:\n  - openapi/buildertrend-openapi.yml\n  - https://developer.buildertrend.com/get-started\n- name: consumerCredentials\n  type: http\n  scheme: basic\n  description: Consumer key as the username, consumer secret as the password (used at POST /api/token). The key and secret may instead be sent as client_id and client_secret form fields.\n  sources:\n  - openapi/buildertrend-openapi.yml\n- name: userSignInPkce\n  type: oauth2\n  declared_in_spec: false\n  flows:\n  - flow: authorizationCode\n    pkce: S256 (RFC 7636)\n    authorizationUrl: https://login.buildertrend.com/authorize\n    tokenUrl: https://login.buildertrend.com/oauth/token\n    audience: https://openapi.buildertrend.net/\n    redirect_uri: http://localhost:8484\n    public_client: true\n    scopes:\n    - openid\n    - profile\n    - email\n    - offline_access\n  token_lifetime:\
  \ access token valid for 24 hours; refresh tokens rotate and last 30 days, or 15 days without use, whichever comes first.\n  description: 'A standard OAuth 2.0 authorization code grant with PKCE (RFC 7636), against\n    Buildertrend''s sign-in service rather than this API. Documented in the OpenAPI info.description,\n    not as a securityScheme. The signing-in user''s account needs Open API access.'\n  sources:\n  - openapi/buildertrend-openapi.yml\nnote: Endpoints read from the published reference; none were called (probe-safety rules forbid token/login calls).\n"
source_yaml_url: https://artifacts.apis.io/buildertrend/authentication/buildertrend-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Construction
- Construction Management
- Residential Construction
- Home Builders
- Remodeling
- Specialty Contractors
- Project Management
- Job Costing
- Estimating
- Scheduling
- CRM
- Proposals
- Change Orders
- Purchase Orders
- Invoicing
- Client Portal
- Subcontractor Portal
- Mobile App
- Software-as-a-Service
- Vertical SaaS
- Construction Technology
---
