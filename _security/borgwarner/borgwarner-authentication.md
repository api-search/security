---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Borgwarner Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: BorgWarner secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: BorgWarner
provider_slug: borgwarner
scheme_count: 2
schemes:
- discovered_via: RFC 8414 authorization server metadata
  flows:
  - authorizationUrl: http://www.borgwarner.com/sitefinity/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    refreshable: true
    scopes: {}
    scopes_note: The metadata document declares no scopes_supported, so there is no scope reference to capture — scopes/ is deliberately not written for this provider.
    tokenUrl: http://www.borgwarner.com/sitefinity/oauth/token
  issuer: http://www.borgwarner.com
  name: sitefinity-oauth2
  observations:
  - The issuer and both endpoint URLs are published as http:// (not https://) in the provider's own metadata document, while the host itself serves and redirects to HTTPS. Recorded verbatim, not corrected.
  - 'GET /sitefinity/oauth/authorize with no parameters returned HTTP 400 "error: invalid_request", confirming a live OAuth authorize endpoint rather than a CMS page.'
  source: https://www.borgwarner.com/.well-known/oauth-authorization-server
  type: oauth2
- discovered_via: WWW-Authenticate challenge on the OData v4 service
  name: sitefinity-odata-bearer
  observed_challenge:
  - 'WWW-Authenticate: Bearer'
  - 'WWW-Authenticate: Cookie realm="https://www.borgwarner.com/", cookie-name=".AspNet.Cookies"'
  protected_resource: https://www.borgwarner.com/api/default
  scheme: bearer
  source: https://www.borgwarner.com/api/default
  status_observed: 401
  type: http
slug: borgwarner-authentication
source_filename: borgwarner-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://www.borgwarner.com/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  There is no OpenAPI in this repo, so derive-authentication.py had nothing to read.\n  This profile is built entirely from responses observed on BorgWarner-controlled hosts\n  on 2026-09-04. SCOPE: both schemes below belong to the Progress Sitefinity CMS that\n  serves www.borgwarner.com — an authenticated-content / site-services surface, not a\n  BorgWarner product API. BorgWarner publishes no developer authentication guide,\n  no key issuance flow and no scope reference.\nsummary:\n  types: [oauth2, http]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  discovery_document: well-known/borgwarner-oauth-authorization-server.json\nschemes:\n  - name: sitefinity-oauth2\n    type: oauth2\n    source: https://www.borgwarner.com/.well-known/oauth-authorization-server\n    discovered_via: RFC 8414 authorization server metadata\n\
  \    issuer: http://www.borgwarner.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: http://www.borgwarner.com/sitefinity/oauth/authorize\n        tokenUrl: http://www.borgwarner.com/sitefinity/oauth/token\n        refreshable: true\n        code_challenge_methods: [S256]\n        scopes: {}\n        scopes_note: >-\n          The metadata document declares no scopes_supported, so there is no scope\n          reference to capture — scopes/ is deliberately not written for this provider.\n    observations:\n      - >-\n        The issuer and both endpoint URLs are published as http:// (not https://) in the\n        provider's own metadata document, while the host itself serves and redirects to\n        HTTPS. Recorded verbatim, not corrected.\n      - >-\n        GET /sitefinity/oauth/authorize with no parameters returned HTTP 400\n        \"error: invalid_request\", confirming a live OAuth authorize endpoint rather\n        than a CMS page.\n  - name: sitefinity-odata-bearer\n\
  \    type: http\n    scheme: bearer\n    source: https://www.borgwarner.com/api/default\n    discovered_via: WWW-Authenticate challenge on the OData v4 service\n    protected_resource: https://www.borgwarner.com/api/default\n    observed_challenge:\n      - 'WWW-Authenticate: Bearer'\n      - 'WWW-Authenticate: Cookie realm=\"https://www.borgwarner.com/\", cookie-name=\".AspNet.Cookies\"'\n    status_observed: 401\nx-evidence:\n  checked: '2026-09-04'\n  probes:\n    - url: https://www.borgwarner.com/.well-known/oauth-authorization-server\n      status: 200\n      content_type: application/json\n    - url: https://www.borgwarner.com/sitefinity/oauth/authorize\n      status: 400\n      body: 'error: invalid_request'\n    - url: https://www.borgwarner.com/api/default/$metadata\n      status: 401\n      content_type: application/json; odata.metadata=minimal\n    - url: https://www.borgwarner.com/.well-known/openid-configuration\n      status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/borgwarner/refs/heads/main/authentication/borgwarner-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Automotive
- Connected Vehicles
- Clean Mobility
- Electric Vehicles
- Propulsion Systems
- Fortune 500
---
