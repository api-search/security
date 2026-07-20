---
api_key_in: []
api_specs:
- filename: fullview-bug-report-openapi.yml
  format: yaml
  label: Fullview Bug Report API
  slug: fullview-bug-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullview/refs/heads/main/openapi/fullview-bug-report-openapi.yml
auth_types:
- openIdConnect
- jwt
description: ''
kind: authentication
layout: security
method: searched
name: Fullview Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
- password
- deviceCode
overview: Fullview secures its APIs with openIdConnect and jwt across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, implicit, password, and deviceCode flow(s).
provider_name: Fullview
provider_slug: fullview
scheme_count: 2
schemes:
- authorization_endpoint: https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/protocol/openid-connect/auth
  grant_types:
  - authorization_code
  - client_credentials
  - implicit
  - password
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  issuer: https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1
  jwks_uri: https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/protocol/openid-connect/certs
  name: fullviewOIDC
  openIdConnectUrl: https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/.well-known/openid-configuration
  provider: Keycloak
  sources:
  - openapi/fullview-bug-report-openapi.yml
  token_endpoint: https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/protocol/openid-connect/token
  type: openIdConnect
- algorithm: RS256
  claims:
    optional:
    - email
    - exp
    - roles
    - env
    - disableReplaysForUser
    - custom
    required:
    - id
    - name
  description: 'Optional end-user identity signing. Your backend signs a JWT (claims: id required, name required, email optional, exp recommended 1 hour, plus optional roles/env/disableReplaysForUser/custom) with a private key; the matching public key is uploaded to Fullview to verify signatures and prevent user impersonation via window.$fvIdentity.'
  docs: https://support.fullview.io/en/articles/15082329-signed-identities-secure-your-users-with-jwt-signed-identities
  key: RSA 2048-bit (or stronger) key pair, PEM format
  name: signedIdentities
  type: jwt
slug: fullview-authentication
source_filename: fullview-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/.well-known/openid-configuration\ndocs: https://support.fullview.io/en/collections/3529098-developer-docs\nsummary:\n  types: [openIdConnect, jwt]\n  oauth2_flows: [authorizationCode, clientCredentials, implicit, password, deviceCode]\n  identity_model: >-\n    Platform authentication uses a Keycloak-based OpenID Connect provider\n    (realm fullview-idp-users-eu1). End-user identity for session replay /\n    cobrowse is established client-side via the window.$fvIdentity object and\n    can be cryptographically secured with RS256 JWT \"Signed Identities\".\nschemes:\n  - name: fullviewOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/.well-known/openid-configuration\n    issuer: https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1\n    authorization_endpoint: https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/protocol/openid-connect/auth\n\
  \    token_endpoint: https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/protocol/openid-connect/token\n    jwks_uri: https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/protocol/openid-connect/certs\n    grant_types: [authorization_code, client_credentials, implicit, password, refresh_token, \"urn:ietf:params:oauth:grant-type:device_code\", \"urn:ietf:params:oauth:grant-type:token-exchange\"]\n    provider: Keycloak\n    sources: [openapi/fullview-bug-report-openapi.yml]\n  - name: signedIdentities\n    type: jwt\n    algorithm: RS256\n    key: RSA 2048-bit (or stronger) key pair, PEM format\n    docs: https://support.fullview.io/en/articles/15082329-signed-identities-secure-your-users-with-jwt-signed-identities\n    description: >-\n      Optional end-user identity signing. Your backend signs a JWT (claims:\n      id required, name required, email optional, exp recommended 1 hour, plus\n      optional roles/env/disableReplaysForUser/custom) with a private key; the\n   \
  \   matching public key is uploaded to Fullview to verify signatures and\n      prevent user impersonation via window.$fvIdentity.\n    claims:\n      required: [id, name]\n      optional: [email, exp, roles, env, disableReplaysForUser, custom]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fullview/refs/heads/main/authentication/fullview-authentication.yml
summary_line: openIdConnect/jwt · 2 schemes
tags:
- Company
- Customer Support
- Cobrowsing
- Session Replay
- Customer Experience
- Developer Tools
- Help Desk
- SaaS
---
