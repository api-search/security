---
api_key_in: []
auth_types:
- cookie-session
- api-token
description: ''
kind: authentication
layout: security
method: probed
name: Voyc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Voyc secures its APIs with cookie-session and api-token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Voyc
provider_slug: voyc
scheme_count: 2
schemes:
- description: The Voyc web application authenticates to /api/v2 with a Django session cookie plus a CSRF double-submit token. The first-party client is configured with withCredentials, xsrfHeaderName "X-CSRFToken" and xsrfCookieName "csrftoken". This is the browser/app path, not a documented integration path.
  evidence:
    detail: 'axios instance created with {withCredentials:true, withXSRFToken:true, xsrfHeaderName:"X-CSRFToken", xsrfCookieName:"csrftoken", baseURL: <api host>/api/v2}'
    source: https://app.voyc.ai/assets/api-Y8KVxUPb.js
  name: SessionCookieWithCSRF
  type: cookie
- description: Voyc API v3 exposes a per-organisation "app" registration with issuable access tokens. The management surface is /v3/organisation/{organisationId}/app/ and /v3/organisation/{organisationId}/app/{appId}/access-token/ (list, create, delete). The token issued there is the credential an integrating system uses. The transport header for the issued token is NOT publicly documented and was not observed unauthenticated.
  evidence:
    detail: First-party app bundle issues GET/POST/PATCH/DELETE against these exact v3 template paths.
    source: https://app.voyc.ai/assets/index-BKkV0m2i.js
  management_endpoints:
  - method: GET
    path: /v3/organisation/{organisationId}/app/
  - method: GET
    path: /v3/organisation/{organisationId}/app/{appId}/
  - method: PATCH
    path: /v3/organisation/{organisationId}/app/{appId}/
  - method: DELETE
    path: /v3/organisation/{organisationId}/app/{appId}/
  - method: GET
    path: /v3/organisation/{organisationId}/app/{appId}/access-token/
  - method: POST
    path: /v3/organisation/{organisationId}/app/{appId}/access-token/
  - method: DELETE
    path: /v3/organisation/{organisationId}/app/{appId}/access-token/{tokenId}/
  name: OrganisationAppAccessToken
  type: apiToken
slug: voyc-authentication
source_filename: voyc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: >-\n  Live unauthenticated probes of https://api.app.voyc.ai plus the public Voyc web\n  application bundle at https://app.voyc.ai/assets/api-Y8KVxUPb.js (first-party\n  JavaScript served from Voyc's own domain).\nnote: >-\n  Voyc publishes no public API reference, so no securityScheme document exists to\n  derive from. This profile is assembled ONLY from what an unauthenticated client\n  can observe on Voyc's own hosts: the HTTP responses api.app.voyc.ai returns, and\n  the request configuration Voyc's own first-party web app ships to every browser.\n  No credentials were used and no access control was defeated.\napi_host: https://api.app.voyc.ai\nsummary:\n  types: [cookie-session, api-token]\n  api_key_in: []\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  public_reference_published: false\nschemes:\n- name: SessionCookieWithCSRF\n  type: cookie\n  description: >-\n    The Voyc web application authenticates\
  \ to /api/v2 with a Django session cookie\n    plus a CSRF double-submit token. The first-party client is configured with\n    withCredentials, xsrfHeaderName \"X-CSRFToken\" and xsrfCookieName \"csrftoken\".\n    This is the browser/app path, not a documented integration path.\n  evidence:\n    source: https://app.voyc.ai/assets/api-Y8KVxUPb.js\n    detail: >-\n      axios instance created with {withCredentials:true, withXSRFToken:true,\n      xsrfHeaderName:\"X-CSRFToken\", xsrfCookieName:\"csrftoken\", baseURL: <api host>/api/v2}\n- name: OrganisationAppAccessToken\n  type: apiToken\n  description: >-\n    Voyc API v3 exposes a per-organisation \"app\" registration with issuable access\n    tokens. The management surface is /v3/organisation/{organisationId}/app/ and\n    /v3/organisation/{organisationId}/app/{appId}/access-token/ (list, create,\n    delete). The token issued there is the credential an integrating system uses.\n    The transport header for the issued token is NOT publicly\
  \ documented and was\n    not observed unauthenticated.\n  management_endpoints:\n  - method: GET\n    path: /v3/organisation/{organisationId}/app/\n  - method: GET\n    path: /v3/organisation/{organisationId}/app/{appId}/\n  - method: PATCH\n    path: /v3/organisation/{organisationId}/app/{appId}/\n  - method: DELETE\n    path: /v3/organisation/{organisationId}/app/{appId}/\n  - method: GET\n    path: /v3/organisation/{organisationId}/app/{appId}/access-token/\n  - method: POST\n    path: /v3/organisation/{organisationId}/app/{appId}/access-token/\n  - method: DELETE\n    path: /v3/organisation/{organisationId}/app/{appId}/access-token/{tokenId}/\n  evidence:\n    source: https://app.voyc.ai/assets/index-BKkV0m2i.js\n    detail: >-\n      First-party app bundle issues GET/POST/PATCH/DELETE against these exact v3\n      template paths.\nobserved_challenges:\n- url: https://api.app.voyc.ai/v3/organisation/\n  method: GET\n  http_status: 403\n  www_authenticate: null\n  body: >-\n    {\"\
  type\":\"client_error\",\"errors\":[{\"code\":\"not_authenticated\",\"detail\":\"Authentication\n    credentials were not provided.\",\"attr\":null}]}\n  detail: >-\n    Returns 403 with a DRF standardized-errors envelope rather than a 401 with a\n    WWW-Authenticate challenge, so an agent gets no machine-readable hint about\n    which credential to present.\n- url: https://api.app.voyc.ai/api/v2/auth/login/\n  method: GET\n  http_status: 200\n  detail: >-\n    Anonymous session-state endpoint; returns {\"authenticated\": false, \"user\": null, ...}\n    to an unauthenticated caller.\ngaps:\n- No public authentication documentation page.\n- No OAuth 2.0 or OpenID Connect surface (/.well-known/oauth-authorization-server,\n  /.well-known/oauth-protected-resource and /.well-known/openid-configuration all 404\n  on api.app.voyc.ai and voyc.ai).\n- The header name and format for the v3 access token are not published, so an\n  integrator cannot write a client from public material.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voyc/refs/heads/main/authentication/voyc-authentication.yml
summary_line: cookie-session/api-token · 2 schemes
tags:
- Company
- Conversation Intelligence
- Compliance
- Call Monitoring
- Speech Analytics
- Contact Centers
- Financial Services
- Artificial Intelligence
---
