---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Enterprise Mobility Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Enterprise Mobility secures its APIs with openIdConnect, oauth2, and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Enterprise Mobility
provider_slug: enterprise-mobility
scheme_count: 3
schemes:
- claims_supported:
  - given_name
  - family_name
  - email
  - signInNames.emailAddress
  - oid
  - idp
  - extension_organizations
  - extension_approved
  - tid
  - iss
  - iat
  - exp
  - aud
  - acr
  - nonce
  - auth_time
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://apimarketplaceprod.b2clogin.com/da7e3fca-e451-444b-9c27-65c9b61e22c2/v2.0/
  name: AzureADB2C
  note: 'The custom claims are the partner gate made visible: extension_organizations carries the organizations a developer is attached to and extension_approved carries the approval flag. Registration is self-serve; API access is not.'
  openIdConnectUrl: https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/B2C_1A_SIGNIN/v2.0/.well-known/openid-configuration
  source: well-known/enterprise-mobility-openid-configuration.json
  subject_types_supported:
  - pairwise
  tenant: apimarketplaceprod.onmicrosoft.com
  type: openIdConnect
- client_id: a76ec3a2-3999-4162-8819-6967df6f7562
  flows:
  - authorizationUrl: https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signin/oauth2/v2.0/authorize
    flow: authorizationCode
    jwksUri: https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signin/discovery/v2.0/keys
    logoutUrl: https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signin/oauth2/v2.0/logout
    policy: B2C_1A_SIGNIN
    scopes_ref: scopes/enterprise-mobility-scopes.yml
    tokenUrl: https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signin/oauth2/v2.0/token
  - authorizationUrl: https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signup/oauth2/v2.0/authorize
    flow: authorizationCode
    jwksUri: https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signup/discovery/v2.0/keys
    logoutUrl: https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signup/oauth2/v2.0/logout
    policy: B2C_1A_SIGNUP
    scopes:
    - openid
    tokenUrl: https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signup/oauth2/v2.0/token
  name: OAuth2AuthorizationCode
  note: client_id and redirect_uri are published verbatim in the anonymous page source of every developer.ehi.com marketplace page. This is a public client identifier, not a secret.
  redirect_uri: https://developer.ehi.com/bin/ehi/auth/code/verifier
  response_modes_supported:
  - query
  - fragment
  - form_post
  response_types_supported:
  - code
  - code id_token
  - code token
  - code id_token token
  - id_token
  - id_token token
  - token
  - token id_token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  type: oauth2
- applies_to: https://api.ehi.com/marketplace/experience/*
  bearerFormat: JWT
  name: BearerToken
  scheme: bearer
  source: '/etc.clientlibs/ehimarketplace/clientlibs/clientlib-site.min.js — every api.ehi.com call sends Authorization: Bearer <access_token>.'
  type: http
slug: enterprise-mobility-authentication
source_filename: enterprise-mobility-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: >-\n  Azure AD B2C OpenID Connect discovery documents (HTTP 200, anonymous), the\n  published sign-in/sign-up authorize links in the developer.ehi.com page source,\n  and the marketplace client library\n  /etc.clientlibs/ehimarketplace/clientlibs/clientlib-site.min.js — all probed\n  2026-07-28.\ndocs: https://developer.ehi.com/\nnote: >-\n  There is no OpenAPI to derive securitySchemes from — the EHI API Marketplace\n  catalog is gated. This profile is assembled entirely from surfaces Enterprise\n  publishes anonymously: the B2C OIDC discovery documents, the authorize URLs\n  embedded in every public marketplace page, and the marketplace's own front-end\n  JavaScript, which shows exactly how it calls api.ehi.com. It describes the\n  identity layer of the marketplace itself. The wire-level auth of the Rental,\n  Replacement Rental and Commute business-line APIs behind the catalog is NOT\n  published and is not asserted here.\n\
  summary:\n  types:\n    - openIdConnect\n    - oauth2\n    - http\n  http_schemes:\n    - bearer\n  oauth2_flows:\n    - authorizationCode\n  api_key_in: []\n  mutual_tls: false\nschemes:\n  - name: AzureADB2C\n    type: openIdConnect\n    openIdConnectUrl: >-\n      https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/B2C_1A_SIGNIN/v2.0/.well-known/openid-configuration\n    source: well-known/enterprise-mobility-openid-configuration.json\n    issuer: https://apimarketplaceprod.b2clogin.com/da7e3fca-e451-444b-9c27-65c9b61e22c2/v2.0/\n    tenant: apimarketplaceprod.onmicrosoft.com\n    id_token_signing_alg_values_supported:\n      - RS256\n    subject_types_supported:\n      - pairwise\n    claims_supported:\n      - given_name\n      - family_name\n      - email\n      - signInNames.emailAddress\n      - oid\n      - idp\n      - extension_organizations\n      - extension_approved\n      - tid\n      - iss\n      - iat\n      - exp\n      - aud\n      - acr\n    \
  \  - nonce\n      - auth_time\n    note: >-\n      The custom claims are the partner gate made visible: extension_organizations\n      carries the organizations a developer is attached to and extension_approved\n      carries the approval flag. Registration is self-serve; API access is not.\n  - name: OAuth2AuthorizationCode\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        policy: B2C_1A_SIGNIN\n        authorizationUrl: >-\n          https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signin/oauth2/v2.0/authorize\n        tokenUrl: >-\n          https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signin/oauth2/v2.0/token\n        logoutUrl: >-\n          https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signin/oauth2/v2.0/logout\n        jwksUri: >-\n          https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signin/discovery/v2.0/keys\n  \
  \      scopes_ref: scopes/enterprise-mobility-scopes.yml\n      - flow: authorizationCode\n        policy: B2C_1A_SIGNUP\n        authorizationUrl: >-\n          https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signup/oauth2/v2.0/authorize\n        tokenUrl: >-\n          https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signup/oauth2/v2.0/token\n        logoutUrl: >-\n          https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signup/oauth2/v2.0/logout\n        jwksUri: >-\n          https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signup/discovery/v2.0/keys\n        scopes:\n          - openid\n    response_types_supported:\n      - code\n      - code id_token\n      - code token\n      - code id_token token\n      - id_token\n      - id_token token\n      - token\n      - token id_token\n    response_modes_supported:\n      - query\n      - fragment\n   \
  \   - form_post\n    token_endpoint_auth_methods_supported:\n      - client_secret_post\n      - client_secret_basic\n    client_id: a76ec3a2-3999-4162-8819-6967df6f7562\n    redirect_uri: https://developer.ehi.com/bin/ehi/auth/code/verifier\n    note: >-\n      client_id and redirect_uri are published verbatim in the anonymous page\n      source of every developer.ehi.com marketplace page. This is a public\n      client identifier, not a secret.\n  - name: BearerToken\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    source: >-\n      /etc.clientlibs/ehimarketplace/clientlibs/clientlib-site.min.js — every\n      api.ehi.com call sends Authorization: Bearer <access_token>.\n    applies_to: https://api.ehi.com/marketplace/experience/*\nadditional_headers:\n  - name: Authorization\n    value: Bearer <access_token>\n    required: true\n    note: B2C-issued access token.\n  - name: ehi-origin-identity\n    value: <id_token>\n    required: true\n    note: >-\n      The B2C id_token\
  \ is sent as a second, EHI-specific identity header\n      alongside the bearer access token.\n  - name: Ehi-Calling-Application\n    value: API Marketplace\n    required: true\n    note: Caller-identification header; the marketplace front end sends its own name.\n  - name: ehi-application-name\n    value: ehi\n    required: false\n    note: Sent on the retrieve-user-content call.\naccess_gate:\n  self_serve_registration: true\n  self_serve_api_access: false\n  requirement: >-\n    \"If you are an Enterprise employee or trusted Partner register and get\n    access today\" — developer.ehi.com. Replacement Rental adds \"Contact your\n    account manager for more information and to request access.\"\n  authorization_step: >-\n    A registered developer creates a Client Application and calls\n    client-application.request-authorization; approval is granted by Enterprise,\n    and surfaces in the token as the extension_approved claim.\nnot_published:\n  - Wire-level authentication for the\
  \ Rental, Replacement Rental and Commute APIs\n  - mTLS / client-certificate requirements, if any\n  - Token lifetimes and refresh semantics\n  - Any API-key scheme\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enterprise-mobility/refs/heads/main/authentication/enterprise-mobility-authentication.yml
summary_line: openIdConnect/oauth2/http · 3 schemes
tags:
- Travel
- United States
- Car Rental
- Ground Transportation
- Mobility
- Corporate Travel
- Distribution
- Fleet Management
- Insurance Replacement Rental
- Booking
---
