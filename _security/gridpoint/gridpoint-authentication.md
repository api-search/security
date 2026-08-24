---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: GridPoint publishes no developer documentation and no OpenAPI, so there is no securityScheme block to derive from. This profile is read entirely from the anonymous OpenID Connect discovery document GridPoint's own authorization server serves, and from the GridPoint Energy Manager application's public JavaScript (window._oauthBaseUrl = "https://identity.gridpoint.com/identity/" in https://ems.gridpoint.com/assets/javascripts/services/apiService.js), which shows the application exchanging and refreshing OAuth 2.0 access/refresh tokens against that endpoint. Nothing here was inferred from marketing copy.
kind: authentication
layout: security
method: probed
name: Gridpoint Authentication
name_suffix: Authentication
oauth_flows: []
overview: GridPoint secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GridPoint
provider_slug: gridpoint
scheme_count: 2
schemes:
- claims:
  - sub
  - email
  - username
  endpoints:
    authorization: https://hydra.gridpoint.com:443/oauth2/auth
    end_session: https://hydra.gridpoint.com:443/oauth2/sessions/logout
    jwks: https://hydra.gridpoint.com:443/.well-known/jwks.json
    registration: https://hydra.gridpoint.com:443/oauth2/clients
    revocation: https://hydra.gridpoint.com:443/oauth2/revoke
    token: https://hydra.gridpoint.com:443/oauth2/token
    userinfo: https://hydra.gridpoint.com:443/userinfo
  features:
    backchannel_logout: true
    dynamic_client_registration: true
    frontchannel_logout: true
    pkce_advertised: false
    request_object_signing: true
    require_request_uri_registration: true
  grant_types:
  - authorization_code
  - implicit
  - client_credentials
  - refresh_token
  id_token_signing_alg_values:
  - RS256
  issuer: https://hydra.gridpoint.com:443/
  name: gridpoint-oidc
  openIdConnectUrl: https://hydra.gridpoint.com/.well-known/openid-configuration
  response_types:
  - code
  - code id_token
  - id_token
  - token id_token
  - token
  - token id_token code
  software: ORY Hydra (self-hosted; identified by the /oauth2/auth, /oauth2/clients and /oauth2/sessions/logout endpoint layout and the health/alive probe)
  sources:
  - well-known/gridpoint-openid-configuration.json
  - well-known/gridpoint-jwks.json
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  - none
  type: openIdConnect
- description: The GridPoint Energy Manager web application (https://ems.gridpoint.com) obtains access_token / refresh_token pairs from https://identity.gridpoint.com/identity/ and stores them client-side, refreshing before expiry. Observed in the application's own unauthenticated JavaScript; the endpoints it calls afterwards are not publicly documented.
  flows:
  - flow: refreshToken
    tokenUrl: https://identity.gridpoint.com/identity/
  name: gridpoint-energy-manager-session
  sources:
  - https://ems.gridpoint.com/assets/javascripts/services/apiService.js
  type: oauth2
slug: gridpoint-authentication
source_filename: gridpoint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://hydra.gridpoint.com/.well-known/openid-configuration\ndocs: null\ndescription: >-\n  GridPoint publishes no developer documentation and no OpenAPI, so there is no\n  securityScheme block to derive from. This profile is read entirely from the\n  anonymous OpenID Connect discovery document GridPoint's own authorization\n  server serves, and from the GridPoint Energy Manager application's public\n  JavaScript (window._oauthBaseUrl = \"https://identity.gridpoint.com/identity/\"\n  in https://ems.gridpoint.com/assets/javascripts/services/apiService.js), which\n  shows the application exchanging and refreshing OAuth 2.0 access/refresh\n  tokens against that endpoint. Nothing here was inferred from marketing copy.\nsummary:\n  types:\n    - oauth2\n    - openIdConnect\n  public_docs: false\n  note: >-\n    An API exists — the authorization server advertises the client_credentials\n    grant and partner/system roles as scopes\
  \ — but the contract it protects is\n    not published. Credentials and reference are both customer/partner-gated.\nschemes:\n  - name: gridpoint-oidc\n    type: openIdConnect\n    openIdConnectUrl: https://hydra.gridpoint.com/.well-known/openid-configuration\n    issuer: https://hydra.gridpoint.com:443/\n    software: ORY Hydra (self-hosted; identified by the /oauth2/auth, /oauth2/clients\n      and /oauth2/sessions/logout endpoint layout and the health/alive probe)\n    endpoints:\n      authorization: https://hydra.gridpoint.com:443/oauth2/auth\n      token: https://hydra.gridpoint.com:443/oauth2/token\n      userinfo: https://hydra.gridpoint.com:443/userinfo\n      jwks: https://hydra.gridpoint.com:443/.well-known/jwks.json\n      registration: https://hydra.gridpoint.com:443/oauth2/clients\n      revocation: https://hydra.gridpoint.com:443/oauth2/revoke\n      end_session: https://hydra.gridpoint.com:443/oauth2/sessions/logout\n    grant_types:\n      - authorization_code\n      -\
  \ implicit\n      - client_credentials\n      - refresh_token\n    response_types:\n      - code\n      - code id_token\n      - id_token\n      - token id_token\n      - token\n      - token id_token code\n    token_endpoint_auth_methods:\n      - client_secret_post\n      - client_secret_basic\n      - private_key_jwt\n      - none\n    id_token_signing_alg_values:\n      - RS256\n    claims:\n      - sub\n      - email\n      - username\n    features:\n      dynamic_client_registration: true\n      pkce_advertised: false\n      backchannel_logout: true\n      frontchannel_logout: true\n      request_object_signing: true\n      require_request_uri_registration: true\n    sources:\n      - well-known/gridpoint-openid-configuration.json\n      - well-known/gridpoint-jwks.json\n  - name: gridpoint-energy-manager-session\n    type: oauth2\n    description: >-\n      The GridPoint Energy Manager web application (https://ems.gridpoint.com)\n      obtains access_token / refresh_token pairs\
  \ from\n      https://identity.gridpoint.com/identity/ and stores them client-side,\n      refreshing before expiry. Observed in the application's own unauthenticated\n      JavaScript; the endpoints it calls afterwards are not publicly documented.\n    flows:\n      - flow: refreshToken\n        tokenUrl: https://identity.gridpoint.com/identity/\n    sources:\n      - https://ems.gridpoint.com/assets/javascripts/services/apiService.js\ngaps:\n  - No public authentication guide, quickstart, or key-issuance page.\n  - No OpenAPI declaring securitySchemes, so scheme-to-operation binding is unknown.\n  - PKCE support is not advertised in discovery (no code_challenge_methods_supported).\n  - No /.well-known/oauth-authorization-server (RFC 8414) or oauth-protected-resource\n    (RFC 9728) document at any host; discovery is OIDC-only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gridpoint/refs/heads/main/authentication/gridpoint-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Energy
- Energy Management
- Buildings
- Building Automation
- Sustainability
- Internet of Things
- Demand Response
- Facilities
- Analytics
---
