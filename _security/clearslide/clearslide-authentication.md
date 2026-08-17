---
api_key_in: []
api_specs:
- filename: clearslide-insights-api-openapi.yml
  format: yaml
  label: ClearSlide Insights API
  slug: clearslide-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-insights-api-openapi.yml
- filename: clearslide-links-api-openapi.yml
  format: yaml
  label: ClearSlide Links API
  slug: clearslide-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-links-api-openapi.yml
- filename: clearslide-meetings-api-openapi.yml
  format: yaml
  label: ClearSlide Meetings API
  slug: clearslide-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-meetings-api-openapi.yml
- filename: clearslide-presentations-api-openapi.yml
  format: yaml
  label: ClearSlide Presentations API
  slug: clearslide-presentations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-presentations-api-openapi.yml
- filename: clearslide-upload-api-openapi.yml
  format: yaml
  label: ClearSlide Upload API
  slug: clearslide-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-upload-api-openapi.yml
- filename: clearslide-users-api-openapi.yml
  format: yaml
  label: ClearSlide Users API
  slug: clearslide-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-users-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Clearslide Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: ClearSlide secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: ClearSlide
provider_slug: clearslide
scheme_count: 1
schemes:
- authorization_server: https://oauth.platform.clearslide.com
  client_authentication:
    detail: client id and client secret base64-encoded in the Authorization header at the token endpoint.
    method: http-basic
    spec: RFC 2617 §2
  description: 'ClearSlide supports the OAuth 2.0 Authorization Code grant (RFC 6749 §4.1) and refresh_token grant. There is no self-service app registration: a partner emails apisupport@clearslide.com with a client redirect URL and is issued a client id and client secret by hand.'
  flows:
  - authorizationUrl: https://oauth.platform.clearslide.com/oauth/authorize
    flow: authorizationCode
    request_params:
    - client_id
    - redirect_uri
    - response_type=code
    - state
    scopes:
    - read
    - write
    tokenUrl: https://oauth.platform.clearslide.com/oauth/token
  - flow: refreshToken
    grant_type: refresh_token
    scopes:
    - read
    - write
    tokenUrl: https://oauth.platform.clearslide.com/oauth/token
  name: oauth2
  sources:
  - https://docs.platform.clearslide.com/oauth2.html
  - https://developer.clearslide.com/docs/oauth-20
  token_request_body: application/x-www-form-urlencoded or application/json
  token_response:
    expires_in_seconds: 3600
    fields:
    - access_token
    - token_type
    - refresh_token
    - Expires_in
    - scope
    note: The documented response field is capitalised `Expires_in`, not the RFC 6749 `expires_in`. Recorded as published.
    token_type: bearer
  type: oauth2
slug: clearslide-authentication
source_filename: clearslide-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://docs.platform.clearslide.com/oauth2.html, https://developer.clearslide.com/docs/oauth-20,\n  https://developer.clearslide.com/docs/scim-at-clearslide,\n  openapi/_original/clearslide-platform-api-swagger.json, and live probes of\n  oauth.platform.clearslide.com and platform.clearslide.com\ndocs: https://developer.clearslide.com/docs/oauth-20\nregistration: mailto:apisupport@clearslide.com\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - refreshToken\n  token_transport: custom-header\n  token_format: opaque UUID\nschemes:\n- name: oauth2\n  type: oauth2\n  authorization_server: https://oauth.platform.clearslide.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.platform.clearslide.com/oauth/authorize\n    tokenUrl: https://oauth.platform.clearslide.com/oauth/token\n    request_params: [client_id, redirect_uri, response_type=code, state]\n    scopes: [read,\
  \ write]\n  - flow: refreshToken\n    tokenUrl: https://oauth.platform.clearslide.com/oauth/token\n    grant_type: refresh_token\n    scopes: [read, write]\n  client_authentication:\n    method: http-basic\n    spec: RFC 2617 §2\n    detail: client id and client secret base64-encoded in the Authorization header at the token endpoint.\n  token_request_body: application/x-www-form-urlencoded or application/json\n  token_response:\n    fields: [access_token, token_type, refresh_token, Expires_in, scope]\n    token_type: bearer\n    expires_in_seconds: 3600\n    note: >-\n      The documented response field is capitalised `Expires_in`, not the RFC 6749 `expires_in`.\n      Recorded as published.\n  description: >-\n    ClearSlide supports the OAuth 2.0 Authorization Code grant (RFC 6749 §4.1) and refresh_token\n    grant. There is no self-service app registration: a partner emails apisupport@clearslide.com\n    with a client redirect URL and is issued a client id and client secret by hand.\n\
  \  sources:\n  - https://docs.platform.clearslide.com/oauth2.html\n  - https://developer.clearslide.com/docs/oauth-20\ntoken_usage:\n- surface: Platform API\n  host: https://platform.clearslide.com\n  header: authorizationToken\n  value: the raw access token\n  bearer_prefix: false\n  rfc6750: false\n  required: true\n  evidence: >-\n    Every one of the six operations in the published Swagger document declares a REQUIRED header\n    parameter named `authorizationToken` with the description \"OAuth2.0 Token\".\n  correction: >-\n    The prior round of this artifact implied a standard `Authorization: Bearer` header. That is\n    wrong for the Platform API and is corrected here.\n- surface: SCIM API\n  host: https://platform.clearslide.com/v2\n  header: authorization\n  value: the access token, shown both bare and with a `Bearer ` prefix in the docs\n  rfc6750: partial\n  evidence: >-\n    The SCIM documentation shows `authorization: xxxxxxxxxxxxxxx` in one example and\n    `-H \"authorization:Bearer\
  \ xxxx\"` in a curl example on the same page.\n  note: Two auth header conventions coexist on one host; the SCIM docs are internally inconsistent about the Bearer prefix.\nimpersonation:\n  header: targetUserId\n  required: true\n  applies_to: [GET /presentations, GET /insights, POST /upload]\n  description: >-\n    A required header naming the user on whose behalf the call operates. Authorisation is\n    therefore a function of the token AND this header, and the contract does not state what\n    constrains which users a given token may target.\nscopes:\n  values: [read, write]\n  granularity: coarse\n  cross_ref: scopes/clearslide-scopes.yml\n  note: >-\n    Two scopes for the entire platform, including SCIM user and group provisioning. There is no\n    scope separating directory administration from content read.\ndiscovery:\n  oauth_authorization_server_metadata: false\n  openid_configuration: false\n  evidence: >-\n    /.well-known/oauth-authorization-server and /.well-known/openid-configuration\
  \ return 404 on\n    every ClearSlide host. Endpoints are only discoverable from prose documentation.\nruntime_evidence:\n  method: probed\n  observations:\n  - url: https://oauth.platform.clearslide.com/oauth/token\n    method: POST\n    status: 401\n    www_authenticate: Basic realm=\"oauth2/client\"\n    server: Apache-Coyote/1.1\n    body_shape: '{timestamp, status, error, message, path}'\n    note: Spring Security OAuth authorization server.\n  - url: https://platform.clearslide.com/presentations\n    method: GET\n    status: 401\n    body: '{\"message\":\"Unauthorized\"}'\n    headers: {x-amzn-errortype: UnauthorizedException}\n    note: AWS API Gateway rejects unauthenticated calls at the edge before ClearSlide code runs.\ngaps:\n- The published contract declares no securityDefinitions, so no generated client can discover the auth model.\n- No PKCE (RFC 7636) is documented for the authorization code flow.\n- No token revocation (RFC 7009) or introspection (RFC 7662) endpoint is\
  \ documented.\n- Onboarding is manual and human-gated, so no agent can obtain credentials programmatically.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/authentication/clearslide-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Sales Engagement
- Sales Enablement
- Content Management
- Presentations
- Analytics
- Meetings
- CRM
- OAuth
- SCIM
---
