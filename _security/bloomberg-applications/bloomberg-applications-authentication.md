---
api_key_in: []
auth_types: []
description: Bloomberg runs three unrelated authentication models across this surface, and which one applies depends entirely on which product a consumer holds. There is no published OpenAPI with securitySchemes, so this profile is assembled from a live 401 challenge on the Data License gateway, the OIDC/OAuth discovery documents bloomberg.com actually serves, and Bloomberg's own BLPAPI Core Developer Guide.
kind: authentication
layout: security
method: searched
name: Bloomberg Applications Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bloomberg Applications declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Bloomberg Applications
provider_slug: bloomberg-applications
scheme_count: 4
schemes:
- applies_to: Bloomberg Data API (Data License / Hypermedia API, api.bloomberg.com/eap)
  bearer_format: JWT
  credential_model: Bloomberg issues a Data License credential object containing client_id, client_secret, name, scopes and creation/expiration dates; the client signs a JWT with it per request. Credentials are provisioned through the Data License contract, not through self-service.
  evidence:
    body: '{"error":"unauthorized_client","error_description":"No definition of jwt found in header or query string.","errors":[{"errorCode":"unauthorized-client","status":401}]}'
    probe: https://api.bloomberg.com/eap/
    status: 401
  id: hapi-jwt
  in: header
  location: Authorization header or query string
  note: An anonymous request to the gateway root returns 403 access_denied; a request to /eap/ returns 401 with the JWT challenge above, which is how the path was confirmed to exist. No anonymous /.well-known/oauth-authorization-server is reachable on this host, so the token endpoint is not machine-discoverable for this API.
  scheme: bearer
  type: http
- applies_to: bloomberg.com account / entitlement checks
  authorization_endpoint: https://login.bloomberg.com/api/oauth/authorize
  evidence:
    probe: https://www.bloomberg.com/.well-known/openid-configuration
    status: 200
  grant_types:
  - authorization_code
  - refresh_token
  id: bloomberg-com-oidc
  id_token_signing_alg: RS256
  issuer: https://www.bloomberg.com
  jwks_uri: https://login.bloomberg.com/api/oauth/.well-known/jwks.json
  note: A genuine, anonymously discoverable OIDC provider. It governs bloomberg.com identity and entitlement, not Data License or BLPAPI data access — do not present it as the API auth path for either.
  openid_connect_url: https://www.bloomberg.com/.well-known/openid-configuration
  pkce: S256
  response_types:
  - code
  scopes:
  - openid
  - user
  - entitlements
  token_endpoint: https://login.bloomberg.com/api/oauth/token
  type: openIdConnect
- applies_to: Bloomberg Terminal Connect API (Desktop API)
  credential_model: No API key. Authorization is inherited from the logged-in Terminal session on the same host; the SDK opens a session against the local Bloomberg Communication Server process.
  id: blpapi-desktop
  in: local socket
  location: 127.0.0.1:8194 on a machine running a logged-in Bloomberg Professional terminal
  note: 'This is why the Desktop API has no public base URL: the endpoint is the operator''s own machine. Failures surface as AuthorizationFailure/NOT_LOGGED_IN and AuthorizationRevoked/INVALID_DISPLAY when the user logs in to a different terminal.'
  type: session
- applies_to: Bloomberg Server API (SAPI) and B-PIPE
  credential_model: Applications authorize through the //blp/apiauth service using a UUID + AuthorizationRequest, an EMRS application name, an IP-based display, or a generated auth token. Entitlements are administered centrally in EMRS (Entitlement Management and Reporting System), and changes there propagate as AUTHORIZATION_STATUS events to live sessions.
  error_codes:
  - INVALID_AUTHTOKEN
  - EXPIRED_AUTHTOKEN
  - TOKEN_IN_USE
  - NOT_LOGGED_ON
  - INVALID_DISPLAY
  - INVALID_USER
  - CROSS_FIRM_AUTH
  - ENTITLEMENTS_MISMATCH
  - CREDENTIAL_REUSE
  - MAX_DEVICES_EXCEEDED
  - MAX_AUTHORIZATIONS_EXCEEDED
  - EMRS_IPRANGE_MISMATCH
  - IP_NOT_IN_RANGE
  id: blpapi-server-bpipe
  note: 'Authorization is revocable mid-session: EMRS administrators can cancel an authorization and the SDK receives AuthorizationRevoked / CANCELLED_BY_SERVER. Clients must handle revocation as a normal runtime event, not an error path.'
  service: //blp/apiauth
  type: token
slug: bloomberg-applications-authentication
source_filename: bloomberg-applications-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  https://www.bloomberg.com/.well-known/openid-configuration (live),\n  https://api.bloomberg.com/eap/ (live 401 challenge),\n  https://data.bloomberglp.com/professional/sites/10/2017/03/BLPAPI-Core-Developer-Guide.pdf\nprovider: Bloomberg Applications\nproviderId: bloomberg-applications\ndescription: >-\n  Bloomberg runs three unrelated authentication models across this surface, and which one\n  applies depends entirely on which product a consumer holds. There is no published OpenAPI\n  with securitySchemes, so this profile is assembled from a live 401 challenge on the Data\n  License gateway, the OIDC/OAuth discovery documents bloomberg.com actually serves, and\n  Bloomberg's own BLPAPI Core Developer Guide.\nschemes:\n  - id: hapi-jwt\n    applies_to: Bloomberg Data API (Data License / Hypermedia API, api.bloomberg.com/eap)\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    in: header\n    location: Authorization\
  \ header or query string\n    evidence:\n      probe: https://api.bloomberg.com/eap/\n      status: 401\n      body: >-\n        {\"error\":\"unauthorized_client\",\"error_description\":\"No definition of jwt found in\n        header or query string.\",\"errors\":[{\"errorCode\":\"unauthorized-client\",\"status\":401}]}\n    credential_model: >-\n      Bloomberg issues a Data License credential object containing client_id, client_secret,\n      name, scopes and creation/expiration dates; the client signs a JWT with it per request.\n      Credentials are provisioned through the Data License contract, not through self-service.\n    note: >-\n      An anonymous request to the gateway root returns 403 access_denied; a request to /eap/\n      returns 401 with the JWT challenge above, which is how the path was confirmed to exist.\n      No anonymous /.well-known/oauth-authorization-server is reachable on this host, so the\n      token endpoint is not machine-discoverable for this API.\n  - id:\
  \ bloomberg-com-oidc\n    applies_to: bloomberg.com account / entitlement checks\n    type: openIdConnect\n    openid_connect_url: https://www.bloomberg.com/.well-known/openid-configuration\n    issuer: https://www.bloomberg.com\n    authorization_endpoint: https://login.bloomberg.com/api/oauth/authorize\n    token_endpoint: https://login.bloomberg.com/api/oauth/token\n    jwks_uri: https://login.bloomberg.com/api/oauth/.well-known/jwks.json\n    grant_types:\n      - authorization_code\n      - refresh_token\n    response_types:\n      - code\n    pkce: S256\n    id_token_signing_alg: RS256\n    scopes:\n      - openid\n      - user\n      - entitlements\n    evidence:\n      probe: https://www.bloomberg.com/.well-known/openid-configuration\n      status: 200\n    note: >-\n      A genuine, anonymously discoverable OIDC provider. It governs bloomberg.com identity and\n      entitlement, not Data License or BLPAPI data access — do not present it as the API auth\n      path for either.\n\
  \  - id: blpapi-desktop\n    applies_to: Bloomberg Terminal Connect API (Desktop API)\n    type: session\n    in: local socket\n    location: 127.0.0.1:8194 on a machine running a logged-in Bloomberg Professional terminal\n    credential_model: >-\n      No API key. Authorization is inherited from the logged-in Terminal session on the same\n      host; the SDK opens a session against the local Bloomberg Communication Server process.\n    note: >-\n      This is why the Desktop API has no public base URL: the endpoint is the operator's own\n      machine. Failures surface as AuthorizationFailure/NOT_LOGGED_IN and\n      AuthorizationRevoked/INVALID_DISPLAY when the user logs in to a different terminal.\n  - id: blpapi-server-bpipe\n    applies_to: Bloomberg Server API (SAPI) and B-PIPE\n    type: token\n    service: //blp/apiauth\n    credential_model: >-\n      Applications authorize through the //blp/apiauth service using a UUID + AuthorizationRequest,\n      an EMRS application name,\
  \ an IP-based display, or a generated auth token. Entitlements are\n      administered centrally in EMRS (Entitlement Management and Reporting System), and changes\n      there propagate as AUTHORIZATION_STATUS events to live sessions.\n    error_codes:\n      - INVALID_AUTHTOKEN\n      - EXPIRED_AUTHTOKEN\n      - TOKEN_IN_USE\n      - NOT_LOGGED_ON\n      - INVALID_DISPLAY\n      - INVALID_USER\n      - CROSS_FIRM_AUTH\n      - ENTITLEMENTS_MISMATCH\n      - CREDENTIAL_REUSE\n      - MAX_DEVICES_EXCEEDED\n      - MAX_AUTHORIZATIONS_EXCEEDED\n      - EMRS_IPRANGE_MISMATCH\n      - IP_NOT_IN_RANGE\n    note: >-\n      Authorization is revocable mid-session: EMRS administrators can cancel an authorization\n      and the SDK receives AuthorizationRevoked / CANCELLED_BY_SERVER. Clients must handle\n      revocation as a normal runtime event, not an error path.\nself_service: false\nonboarding: >-\n  No self-service signup exists for any of these. Data License credentials and B-PIPE/SAPI\n\
  \  entitlements are provisioned under contract; developer.bloomberg.com requires an existing\n  Bloomberg account to reach any reference documentation.\ndocs:\n  - https://professional.bloomberg.com/support/api-library/\n  - https://data.bloomberglp.com/professional/sites/10/2017/03/BLPAPI-Core-Developer-Guide.pdf\n  - https://developer.bloomberg.com/\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-applications/refs/heads/main/authentication/bloomberg-applications-authentication.yml
summary_line: 4 schemes
tags:
- Enterprise API
- Financial Analytics
- Financial-Services
- Market Data
- Real-Time Data
---
