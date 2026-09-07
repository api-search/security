---
anonymous_access: false
api_key_in: []
api_specs:
- filename: canvas-lms-openapi.yml
  format: yaml
  label: Canvas LMS REST API
  slug: canvas-lms-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canvas/refs/heads/main/openapi/canvas-lms-openapi.yml
- filename: canvas-courses-api-openapi.yml
  format: yaml
  label: Canvas Courses API
  slug: canvas-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canvas/refs/heads/main/openapi/canvas-courses-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Canvas Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Canvas secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Canvas
provider_slug: canvas
scheme_count: 2
schemes:
- description: 'Canvas OAuth2 access token sent as "Authorization: Bearer <token>". See https://canvas.instructure.com/doc/api/file.oauth.html'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/canvas-courses-api-openapi.yml
  - openapi/canvas-lms-openapi.yml
  type: http
- description: Canvas OAuth2. See https://canvas.instructure.com/doc/api/file.oauth.html and https://canvas.instructure.com/doc/api/file.oauth_endpoints.html
  flows:
  - authorizationUrl: https://canvas.instructure.com/login/oauth2/auth
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://canvas.instructure.com/login/oauth2/token
  name: oauth2
  sources:
  - openapi/canvas-courses-api-openapi.yml
  - openapi/canvas-lms-openapi.yml
  type: oauth2
slug: canvas-authentication
source_filename: canvas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: openapi/canvas-courses-api-openapi.yml, openapi/canvas-lms-openapi.yml + Instructure OAuth2 documentation\n  (searched 2026-09-05)\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Canvas OAuth2 access token sent as \"Authorization: Bearer <token>\". See https://canvas.instructure.com/doc/api/file.oauth.html'\n  sources:\n  - openapi/canvas-courses-api-openapi.yml\n  - openapi/canvas-lms-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://canvas.instructure.com/login/oauth2/auth\n    tokenUrl: https://canvas.instructure.com/login/oauth2/token\n    scopes: 0\n  description: Canvas OAuth2. See https://canvas.instructure.com/doc/api/file.oauth.html and https://canvas.instructure.com/doc/api/file.oauth_endpoints.html\n  sources:\n  - openapi/canvas-courses-api-openapi.yml\n\
  \  - openapi/canvas-lms-openapi.yml\ndocs:\n- https://developerdocs.instructure.com/services/canvas/oauth2/file.oauth\n- https://developerdocs.instructure.com/services/canvas/oauth2/file.oauth_endpoints\n- https://developerdocs.instructure.com/services/canvas/oauth2/file.developer_keys\n- https://developerdocs.instructure.com/services/canvas/resources/api_token_scopes\nmodel: OAuth 2.0 (RFC 6749) authorization code, plus manually generated personal access tokens\nendpoints:\n  authorize:\n    method: GET\n    url: https://<canvas-host>/login/oauth2/auth\n    params:\n    - client_id\n    - response_type=code\n    - redirect_uri\n    - state\n    - scope\n    - purpose\n    - force_login\n    - unique_id\n    - prompt=none\n  token:\n    method: POST\n    url: https://<canvas-host>/login/oauth2/token\n    grant_types:\n    - authorization_code\n    - refresh_token\n    - client_credentials\n    note: client_credentials is used for LTI Advantage service tokens, signed with the tool's JWK\
  \ — not for the\n      Canvas REST API.\n  logout:\n    method: DELETE\n    url: https://<canvas-host>/login/oauth2/token\n    note: Expires the access token. `expire_sessions=1` also ends the user's Canvas web sessions.\n  session_token:\n    method: GET\n    url: https://<canvas-host>/login/session_token\n    note: Exchanges an API token for a one-time URL that logs the user into the Canvas web UI.\ntoken_lifetime:\n  access_token: 1 hour (developer keys issued after Oct 2015)\n  refresh_token: long-lived\n  note: Applications MUST implement refresh; there is no long-lived access token for OAuth apps.\nmanual_tokens:\n  where: /profile → Approved Integrations → New Access Token\n  shown_once: true\n  policy: Instructure's Canvas API Policy forbids asking another user to generate and hand over a token. Multi-user\n    applications must use OAuth. https://www.instructure.com/policies/canvas-api-policy\ndeveloper_keys:\n  issued_by: the institution's Canvas admin (Site Admin on a self-hosted\
  \ install)\n  scoping: Keys are scoped to the institution that issued them. A tool serving many institutions must store one\n    key per Canvas domain and pick it from the launch context (custom_canvas_api_domain).\n  enforce_scopes: Optional per key. When off, the key grants everything its user can do.\n  docs: https://developerdocs.instructure.com/services/canvas/oauth2/file.developer_keys\nscopes:\n  model: per-endpoint strings of the form url:<VERB>|/api/v1/<path>\n  see: scopes/canvas-scopes.yml\n  identity_only: /auth/userinfo returns the user's name and id and no access token.\nerror_signals:\n  401_with_www_authenticate: token invalid, expired, or issued on a different Canvas host\n  401_without_www_authenticate: authenticated but not permitted\n  see: errors/canvas-problem-types.yml\nidentity_federation:\n  note: 'Separately from API auth, Canvas federates END-USER login through the Authentication Providers resource:\n    SAML 2.0, CAS, LDAP and OpenID Connect.'\n  see: conformance/canvas-conformance.yml\n\
  lti_advantage:\n  note: LTI 1.3 tools authenticate to Canvas services with a signed JWT client-credentials grant, per the 1EdTech\n    Security Framework — not with a Canvas API token.\n  docs: https://developerdocs.instructure.com/services/canvas/external-tools/lti/file.tools_intro\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canvas/refs/heads/main/authentication/canvas-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Education
- EdTech
- GraphQL
- Learning Management System
- LMS
- LTI
- Open-Source
- REST
---
