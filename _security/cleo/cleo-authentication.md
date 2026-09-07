---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Cleo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Cleo secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Cleo
provider_slug: cleo
scheme_count: 1
schemes:
- code_challenge_methods_supported:
  - S256
  flows:
  - authorizationUrl: https://www.meetcleo.com/oauth/authorize
    flow: authorizationCode
    scopes:
    - read
    - write:create
    - write:delete
    tokenUrl: https://www.meetcleo.com/oauth/token
  - flow: refreshToken
    tokenUrl: https://www.meetcleo.com/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://www.meetcleo.com
  name: OAuth2
  response_types_supported:
  - code
  source: https://www.meetcleo.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: cleo-authentication
source_filename: cleo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://www.meetcleo.com/.well-known/oauth-authorization-server\nnote: >-\n  Cleo publishes no OpenAPI, so this profile is not derived from a spec. It is read\n  verbatim from the one machine-readable authorization document Cleo serves publicly:\n  an RFC 8414 OAuth 2.0 Authorization Server Metadata document at\n  https://www.meetcleo.com/.well-known/oauth-authorization-server (HTTP 200,\n  application/json, issuer https://www.meetcleo.com).\nscope_of_this_record: >-\n  IMPORTANT — this is NOT a third-party developer authorization surface. A GET of the\n  advertised authorization_endpoint (https://www.meetcleo.com/oauth/authorize) returns\n  302 to https://www.meetcleo.com/admin_log_in, an internal administrative sign-in.\n  Cleo runs no public developer program and issues no third-party API credentials, so\n  the metadata below documents an internal/administrative OAuth deployment that happens\n  to be discoverable at the standard\
  \ well-known path. It is recorded because it is real\n  and published, not because it is callable by an outside integrator.\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken]\n  public_client: true\n  pkce_required_methods: [S256]\n  dynamic_client_registration: false\n  openid_connect: false\nschemes:\n  - name: OAuth2\n    type: oauth2\n    issuer: https://www.meetcleo.com\n    source: https://www.meetcleo.com/.well-known/oauth-authorization-server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://www.meetcleo.com/oauth/authorize\n        tokenUrl: https://www.meetcleo.com/oauth/token\n        scopes: [read, 'write:create', 'write:delete']\n      - flow: refreshToken\n        tokenUrl: https://www.meetcleo.com/oauth/token\n    token_endpoint_auth_methods_supported: [none]\n    code_challenge_methods_supported: [S256]\n    response_types_supported: [code]\n    grant_types_supported: [authorization_code, refresh_token]\n\
  observations:\n  - >-\n    token_endpoint_auth_methods_supported is [\"none\"], which with PKCE S256 is the\n    public-client profile — the deployment expects clients that cannot hold a secret.\n  - >-\n    No registration_endpoint is advertised, so there is no RFC 7591 dynamic client\n    registration; clients must be provisioned out of band.\n  - >-\n    No /.well-known/openid-configuration is served (404 on every host probed), so this\n    is plain OAuth 2.0, not OpenID Connect.\n  - >-\n    No jwks_uri, introspection_endpoint or revocation_endpoint is advertised.\nx-evidence:\n  - url: https://www.meetcleo.com/.well-known/oauth-authorization-server\n    http_status: 200\n    content_type: application/json; charset=utf-8\n    fetched: '2026-09-05'\n  - url: https://www.meetcleo.com/oauth/authorize\n    http_status: 302\n    location: https://www.meetcleo.com/admin_log_in\n    fetched: '2026-09-05'\n  - url: https://www.meetcleo.com/.well-known/openid-configuration\n    http_status:\
  \ 404\n    fetched: '2026-09-05'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cleo/refs/heads/main/authentication/cleo-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Artificial Intelligence
- Banking
- Budgeting
- Cash Advance
- Consumer Finance
- Financial Assistant
- Personal Finance
---
