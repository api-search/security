---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: dotcms-rest-api-openapi.json
  format: json
  label: dotCMS REST API
  slug: rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotcms/refs/heads/main/openapi/dotcms-rest-api-openapi.json
auth_types:
- http
- apiKey-as-bearer
- session
description: 'Authentication profile for the dotCMS REST and GraphQL APIs, sourced from the provider''s own auth documentation. It is `searched` rather than `derived` for a specific reason worth recording: the first-party OpenAPI dotCMS serves at /api/openapi.json declares NO components.securitySchemes and no top-level security requirement, across all 754 operations — while 368 of those operations declare a 401 response. The contract knows auth is required and does not say what it is. Everything below therefore comes from the docs, not from the spec.'
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Dotcms Authentication
name_suffix: Authentication
oauth_flows: []
overview: dotCMS secures its APIs with http, apiKey-as-bearer, and session across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: dotCMS
provider_slug: dotcms
scheme_count: 5
schemes:
- bearerFormat: JWT
  expiry: Set per token at mint time via expirationDays; tokens are stateless JWTs.
  format: 'Authorization: Bearer <token>'
  header: Authorization
  mint:
    body_fields:
    - user
    - password
    - expirationDays
    example_shape: '{"user":"<email>","password":"<password>","expirationDays":10}'
    operation: POST /api/v1/authentication/api-token
    operationId: requestApiToken
  name: APIToken
  note: The recommended method, and the one the dotCMS MCP server and dotCLI both use. The MCP server reads it from AUTH_TOKEN and its docs require write permission on Content Types, Content and Workflows.
  primary: true
  scheme: bearer
  source: docs
  type: http
  ui_mint: System > Users > API Access Tokens
- format: 'AUTHENTICATION: <base64(user:password)>'
  header: AUTHENTICATION
  name: BasicAuth
  note: 'Note the non-standard header name — dotCMS uses AUTHENTICATION, not Authorization, for this mode. The docs warn: "Base64 encoding does not encrypt the user name and password." HTTPS only.'
  scheme: basic
  source: docs
  type: http
- format: 'DOTAUTH: <base64(user:password)>'
  header: DOTAUTH
  name: DOTAUTH
  note: dotCMS-specific alias for basic auth. Security by obscurity only.
  scheme: basic-variant
  source: docs
  type: http
- name: SessionCookie
  note: Established by logging into the dotCMS back end or front end; both back-end and front-end user roles are supported. Relevant to browser-embedded calls, not to server-to-server agents.
  source: docs
  type: session
- discouraged: true
  format: /user/xxx/password/yyy
  name: URLParameters
  note: Documented for legacy compatibility and explicitly the least secure option — credentials appear in access logs, proxies and browser history. Never use from an agent.
  source: docs
  type: query
slug: dotcms-authentication
source_filename: dotcms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://dev.dotcms.com/docs/build/apis/api-basics/rest-api-authentication\ndocs: https://dev.dotcms.com/docs/build/apis/api-basics/rest-api-authentication\nspec_reference: openapi/dotcms-rest-api-openapi.json\ndescription: >-\n  Authentication profile for the dotCMS REST and GraphQL APIs, sourced from the provider's own\n  auth documentation. It is `searched` rather than `derived` for a specific reason worth\n  recording: the first-party OpenAPI dotCMS serves at /api/openapi.json declares NO\n  components.securitySchemes and no top-level security requirement, across all 754 operations —\n  while 368 of those operations declare a 401 response. The contract knows auth is required and\n  does not say what it is. Everything below therefore comes from the docs, not from the spec.\nspec_gap:\n  security_schemes_declared: 0\n  operations_declaring_401: 368\n  operations_declaring_403: 348\n  impact: >-\n    A client generated from\
  \ this spec ships with no authentication wiring at all. This is the\n    single highest-leverage contract fix available to dotCMS: adding a bearerAuth securityScheme\n    plus a top-level security block would cost a few lines and would make every generated SDK\n    and every agent tool-call correct by construction.\nsummary:\n  types: [http, apiKey-as-bearer, session]\n  api_key_in: [header]\n  oauth2_flows: []\n  primary: bearer-jwt\nschemes:\n- name: APIToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  primary: true\n  header: Authorization\n  format: 'Authorization: Bearer <token>'\n  mint:\n    operation: POST /api/v1/authentication/api-token\n    operationId: requestApiToken\n    body_fields: [user, password, expirationDays]\n    example_shape: '{\"user\":\"<email>\",\"password\":\"<password>\",\"expirationDays\":10}'\n  ui_mint: System > Users > API Access Tokens\n  expiry: Set per token at mint time via expirationDays; tokens are stateless JWTs.\n  source: docs\n  note:\
  \ >-\n    The recommended method, and the one the dotCMS MCP server and dotCLI both use. The MCP server\n    reads it from AUTH_TOKEN and its docs require write permission on Content Types, Content and\n    Workflows.\n- name: BasicAuth\n  type: http\n  scheme: basic\n  header: AUTHENTICATION\n  format: 'AUTHENTICATION: <base64(user:password)>'\n  source: docs\n  note: >-\n    Note the non-standard header name — dotCMS uses AUTHENTICATION, not Authorization, for this\n    mode. The docs warn: \"Base64 encoding does not encrypt the user name and password.\" HTTPS\n    only.\n- name: DOTAUTH\n  type: http\n  scheme: basic-variant\n  header: DOTAUTH\n  format: 'DOTAUTH: <base64(user:password)>'\n  source: docs\n  note: dotCMS-specific alias for basic auth. Security by obscurity only.\n- name: SessionCookie\n  type: session\n  source: docs\n  note: >-\n    Established by logging into the dotCMS back end or front end; both back-end and front-end\n    user roles are supported. Relevant to browser-embedded\
  \ calls, not to server-to-server agents.\n- name: URLParameters\n  type: query\n  format: /user/xxx/password/yyy\n  discouraged: true\n  source: docs\n  note: >-\n    Documented for legacy compatibility and explicitly the least secure option — credentials\n    appear in access logs, proxies and browser history. Never use from an agent.\nend_user_sso:\n  note: >-\n    Distinct from API authentication. dotCMS configures OAuth/OIDC and SAML for END-USER login to\n    the platform, per site, under the `dotAuth` (15 operations) and `SAML Authentication` tags in\n    the spec. These are configuration endpoints for identity federation, not an OAuth\n    authorization surface for the API itself — which is why no scopes/ artifact is emitted: the\n    dotCMS API has no OAuth scope model. Authorization is by dotCMS role and per-asset\n    permission, evaluated server-side against the token's user.\n  spec_tags: [dotAuth, \"SAML Authentication\"]\n  operations: 15\nauthorization_model:\n  kind: rbac-plus-acl\n\
  \  note: >-\n    dotCMS authorizes by role membership plus per-asset permissions rather than by token scope.\n    17 operations declare \"Forbidden - CMS Administrator role required\" and 8 declare \"User lacks\n    the Scripting Developer role\" — the roles are named in the contract's response descriptions\n    even though they are not modelled as scopes. Successful responses echo the caller's rights\n    back in the envelope's `permissions[]` array, which is a genuinely useful runtime signal for\n    an agent deciding whether to attempt a write.\n  runtime_signal: response envelope `permissions[]`\nrevocation:\n  documented: false\n  note: >-\n    Tokens are revocable through the dotCMS admin UI (API Access Tokens tab). No REST revocation\n    endpoint is documented on the auth page; expirationDays is the primary control.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dotcms/refs/heads/main/authentication/dotcms-authentication.yml
summary_line: http/apiKey-as-bearer/session · 5 schemes
tags:
- CMS
- Content
- Content Management
- Headless CMS
- Digital Experience
- Content Delivery
- Workflows
- GraphQL
- MCP
- Java
---
