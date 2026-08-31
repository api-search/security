---
api_key_in: []
api_specs:
- filename: propertyme-connection-api-openapi.yml
  format: yaml
  label: PropertyMe Connection API
  slug: propertyme-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-connection-api-openapi.yml
- filename: propertyme-scope-activities-api-openapi.yml
  format: yaml
  label: 'PropertyMe Scope: Activities API'
  slug: propertyme-scope-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-scope-activities-api-openapi.yml
- filename: propertyme-scope-bills-api-openapi.yml
  format: yaml
  label: 'PropertyMe Scope: Bills API'
  slug: propertyme-scope-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-scope-bills-api-openapi.yml
- filename: propertyme-scope-contacts-api-openapi.yml
  format: yaml
  label: 'PropertyMe Scope: Contacts API'
  slug: propertyme-scope-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-scope-contacts-api-openapi.yml
- filename: propertyme-scope-messages-api-openapi.yml
  format: yaml
  label: 'PropertyMe Scope: Messages API'
  slug: propertyme-scope-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-scope-messages-api-openapi.yml
- filename: propertyme-scope-properties-api-openapi.yml
  format: yaml
  label: 'PropertyMe Scope: Properties API'
  slug: propertyme-scope-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-scope-properties-api-openapi.yml
auth_types:
- openIdConnect
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Propertyme Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
- password
- deviceCode
- ciba
- refreshToken
overview: PropertyMe secures its APIs with openIdConnect, oauth2, and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, implicit, password, deviceCode, ciba, and refreshToken flow(s).
provider_name: PropertyMe
provider_slug: propertyme
scheme_count: 2
schemes:
- client_auth_methods:
  - client_secret_basic
  - client_secret_post
  dpop_signing_alg_values:
  - RS256
  - RS384
  - RS512
  - PS256
  - PS384
  - PS512
  - ES256
  - ES384
  - ES512
  endpoints:
    authorization: https://login.propertyme.com/connect/authorize
    backchannel_authentication: https://login.propertyme.com/connect/ciba
    check_session: https://login.propertyme.com/connect/checksession
    device_authorization: https://login.propertyme.com/connect/deviceauthorization
    end_session: https://login.propertyme.com/connect/endsession
    introspection: https://login.propertyme.com/connect/introspect
    pushed_authorization_request: https://login.propertyme.com/connect/par
    registration: https://login.propertyme.com/connect/dcr
    revocation: https://login.propertyme.com/connect/revocation
    token: https://login.propertyme.com/connect/token
    userinfo: https://login.propertyme.com/connect/userinfo
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  - mcp_customer_switch
  - on_behalf_of
  id_token_signing_alg:
  - RS256
  issuer: https://login.propertyme.com
  jwks_uri: https://login.propertyme.com/.well-known/openid-configuration/jwks
  name: PropertyMeOIDC
  openIdConnectUrl: https://login.propertyme.com/.well-known/openid-configuration
  prompt_values:
  - none
  - login
  - consent
  - select_account
  require_pushed_authorization_requests: false
  scopes_ref: scopes/propertyme-scopes.yml
  sources:
  - https://login.propertyme.com/.well-known/openid-configuration
  subject_types:
  - public
  type: openIdConnect
- in: header
  name: Bearer
  note: Declared in the Swagger document as type apiKey with name Authorization in header. This is a Swashbuckle description of an OIDC bearer token, not a static API key — PropertyMe issues no long-lived API keys.
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/propertyme-openapi.json
  type: http
slug: propertyme-authentication
source_filename: propertyme-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: https://login.propertyme.com/.well-known/openid-configuration\nsupplemental_source: openapi/propertyme-openapi.json\ndocs: https://github.com/PropertyMe/HelloPropertyMe.NET\nnotes: >-\n  The Swagger 2.0 contract understates PropertyMe's auth model badly: it declares one `Bearer`\n  securityDefinition typed `apiKey` in the Authorization header, which is how a great many .NET\n  Swashbuckle documents describe a bearer token. The real model is full OpenID Connect on an\n  IdentityServer-family deployment at login.propertyme.com, whose discovery document is served\n  anonymously and is unusually complete — PAR, DPoP signing algorithms, CIBA backchannel auth, device\n  code, front- and back-channel logout, token revocation and introspection, and dynamic client\n  registration at /connect/dcr. Two non-standard grant types are advertised: `mcp_customer_switch`\n  and `on_behalf_of`. The gate is not the protocol, it is issuance — there\
  \ is no self-serve developer\n  signup anywhere on propertyme.com.au or app.propertyme.com, and no developer/docs/api subdomain\n  resolves, so a client_id and client_secret must be issued by PropertyMe directly. Every issued\n  token is additionally scoped to the single customer portfolio the agency has connected, and the\n  agency can sever that connection at any time.\nsummary:\n  types: [openIdConnect, oauth2, http]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials, implicit, password, deviceCode, ciba, refreshToken]\n  token_placement: 'Authorization: Bearer <access_token>'\n  pkce: [S256, plain]\n  self_serve_registration: false\n  dynamic_client_registration_endpoint: https://login.propertyme.com/connect/dcr\nschemes:\n  - name: PropertyMeOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://login.propertyme.com/.well-known/openid-configuration\n    issuer: https://login.propertyme.com\n    jwks_uri: https://login.propertyme.com/.well-known/openid-configuration/jwks\n\
  \    id_token_signing_alg: [RS256]\n    subject_types: [public]\n    sources: [https://login.propertyme.com/.well-known/openid-configuration]\n    endpoints:\n      authorization: https://login.propertyme.com/connect/authorize\n      token: https://login.propertyme.com/connect/token\n      userinfo: https://login.propertyme.com/connect/userinfo\n      introspection: https://login.propertyme.com/connect/introspect\n      revocation: https://login.propertyme.com/connect/revocation\n      end_session: https://login.propertyme.com/connect/endsession\n      check_session: https://login.propertyme.com/connect/checksession\n      device_authorization: https://login.propertyme.com/connect/deviceauthorization\n      backchannel_authentication: https://login.propertyme.com/connect/ciba\n      pushed_authorization_request: https://login.propertyme.com/connect/par\n      registration: https://login.propertyme.com/connect/dcr\n    grant_types:\n      - authorization_code\n      - client_credentials\n\
  \      - refresh_token\n      - implicit\n      - password\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:openid:params:grant-type:ciba\n      - mcp_customer_switch\n      - on_behalf_of\n    client_auth_methods: [client_secret_basic, client_secret_post]\n    require_pushed_authorization_requests: false\n    dpop_signing_alg_values: [RS256, RS384, RS512, PS256, PS384, PS512, ES256, ES384, ES512]\n    prompt_values: [none, login, consent, select_account]\n    scopes_ref: scopes/propertyme-scopes.yml\n  - name: Bearer\n    type: http\n    scheme: bearer\n    in: header\n    parameter: Authorization\n    sources: [openapi/propertyme-openapi.json]\n    note: >-\n      Declared in the Swagger document as type apiKey with name Authorization in header. This is a\n      Swashbuckle description of an OIDC bearer token, not a static API key — PropertyMe issues no\n      long-lived API keys.\nconsent:\n  model: per-customer portfolio connection\n  granularity: one connected portfolio\
  \ per integration per agency\n  revocation:\n    by_agency: The agency disconnects the integration from within PropertyMe.\n    by_integration: DELETE /v1/portfolios/disconnect\n    note: Disconnecting invalidates the current access token; the portfolio user must choose to reconnect.\nnon_standard_grants:\n  - grant: mcp_customer_switch\n    observed: https://login.propertyme.com/.well-known/openid-configuration\n    reading: >-\n      Switches the acting customer portfolio for an already-authenticated session. Strong evidence of\n      an internal Model Context Protocol surface — see mcp/propertyme-mcp.yml.\n  - grant: on_behalf_of\n    observed: https://login.propertyme.com/.well-known/openid-configuration\n    reading: Token exchange so a service can act for a specific user or customer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/authentication/propertyme-authentication.yml
summary_line: openIdConnect/oauth2/http · 2 schemes
tags:
- Real-Estate
- Australia
- Property Management
- Rentals
- PropTech
- Tenancy
- Trust Accounting
- Inspections
- Maintenance
- Documents
- Payments
- New Zealand
---
