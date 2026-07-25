---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Cohere Health Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- refreshToken
- implicit
- password
overview: Cohere Health secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, refreshToken, implicit, and password flow(s).
provider_name: Cohere Health
provider_slug: cohere-health
scheme_count: 2
schemes:
- code_challenge_methods_supported:
  - S256
  endpoints:
    authorization: https://login.coherehealth.com/oauth2/v1/authorize
    device_authorization: https://login.coherehealth.com/oauth2/v1/device/authorize
    end_session: https://login.coherehealth.com/oauth2/v1/logout
    introspection: https://login.coherehealth.com/oauth2/v1/introspect
    jwks: https://login.coherehealth.com/oauth2/v1/keys
    registration: https://login.coherehealth.com/oauth2/v1/clients
    revocation: https://login.coherehealth.com/oauth2/v1/revoke
    token: https://login.coherehealth.com/oauth2/v1/token
    userinfo: https://login.coherehealth.com/oauth2/v1/userinfo
  grant_types_supported:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  issuer: https://login.coherehealth.com
  name: OpenIDConnect
  openIdConnectUrl: https://login.coherehealth.com/.well-known/openid-configuration
  sources:
  - well-known/cohere-health-openid-configuration.json
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
- documented: true
  name: SMARTonFHIR
  note: The CRD, DTR and PAS APIs are documented as supporting SMART on FHIR applications (OAuth2 authorization-code and/or client-credentials with patient/*, user/* or system/* scopes per the Da Vinci CRD/DTR/PAS implementation guides). Endpoints and scopes are per-health-plan tenant and not anonymously served, so no concrete scheme is asserted here.
  published: false
  sources:
  - https://www.coherehealth.com/utilization-management/api-based
  type: oauth2
slug: cohere-health-authentication
source_filename: cohere-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://login.coherehealth.com/.well-known/openid-configuration\nnote: >-\n  Auth profile captured from the live OIDC discovery document served by the\n  Cohere platform login host (login.coherehealth.com, an Okta-backed identity\n  tenant). This governs authentication to the Cohere Unify platform / provider\n  portal. The CRD/DTR/PAS FHIR APIs are documented as SMART-on-FHIR (OAuth2)\n  applications, but their concrete authorize/token endpoints and scopes are\n  provisioned per health-plan tenant and are not published anonymously.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, clientCredentials, deviceCode, refreshToken, implicit, password]\n  pkce: S256\n  identity_provider: Okta\nschemes:\n  - name: OpenIDConnect\n    type: openIdConnect\n    openIdConnectUrl: https://login.coherehealth.com/.well-known/openid-configuration\n    issuer: https://login.coherehealth.com\n    endpoints:\n   \
  \   authorization: https://login.coherehealth.com/oauth2/v1/authorize\n      token: https://login.coherehealth.com/oauth2/v1/token\n      userinfo: https://login.coherehealth.com/oauth2/v1/userinfo\n      jwks: https://login.coherehealth.com/oauth2/v1/keys\n      registration: https://login.coherehealth.com/oauth2/v1/clients\n      introspection: https://login.coherehealth.com/oauth2/v1/introspect\n      revocation: https://login.coherehealth.com/oauth2/v1/revoke\n      device_authorization: https://login.coherehealth.com/oauth2/v1/device/authorize\n      end_session: https://login.coherehealth.com/oauth2/v1/logout\n    grant_types_supported: [authorization_code, implicit, refresh_token, password, urn:ietf:params:oauth:grant-type:device_code]\n    token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, client_secret_jwt, private_key_jwt, none]\n    code_challenge_methods_supported: [S256]\n    sources: [well-known/cohere-health-openid-configuration.json]\n  - name:\
  \ SMARTonFHIR\n    type: oauth2\n    documented: true\n    published: false\n    note: >-\n      The CRD, DTR and PAS APIs are documented as supporting SMART on FHIR\n      applications (OAuth2 authorization-code and/or client-credentials with\n      patient/*, user/* or system/* scopes per the Da Vinci CRD/DTR/PAS\n      implementation guides). Endpoints and scopes are per-health-plan tenant\n      and not anonymously served, so no concrete scheme is asserted here.\n    sources: [https://www.coherehealth.com/utilization-management/api-based]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cohere-health/refs/heads/main/authentication/cohere-health-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Healthcare
- United States
- Prior Authorization
- Utilization Management
- Payer
- FHIR
- HL7
- Da Vinci
- SMART on FHIR
- Interoperability
---
