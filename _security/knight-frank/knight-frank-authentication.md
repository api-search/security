---
api_key_in: []
api_specs:
- filename: knight-frank-api-v3-openapi.json
  format: json
  label: KnightFrank Api v3
  slug: knight-frank-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knight-frank/refs/heads/main/openapi/knight-frank-api-v3-openapi.json
auth_types:
- none
- oauth2
- openIdConnect
description: Knight Frank runs two authentication postures at once and neither is a developer credential. The corporate search service (api-v3) enforces NO authentication at all — its OpenAPI declares no securitySchemes, sends no security requirement, and answers anonymous GETs with real office and people-directory records. The property/account service (api-v2) is fully closed — every request without a bearer token returns 401 — and is protected by Azure AD B2C through a first-party MSAL client belonging to the consumer "My Knight Frank" saved-property account. There is no API key programme, no client-credentials flow, no developer application registration and no way for a third party to obtain a credential of any kind.
kind: authentication
layout: security
method: searched
name: Knight Frank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Knight Frank secures its APIs with none, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Knight Frank
provider_slug: knight-frank
scheme_count: 2
schemes:
- detail: 'The harvested OpenAPI 3.0.1 document contains no components.securitySchemes block and no security array. Verified live on 2026-07-26: GET /office, GET /office/{id}, GET /person, GET /person/autocomplete, GET /person/cms-search, GET /search, GET /cmspage, GET /intelligencelab and GET /service-lines all returned HTTP 200 with real JSON to a client presenting no credential.'
  evidence:
  - request: GET https://api-v3.web.prd-knightfrank.com/office?term=london&isoCode=GB&languageCode=en&maxResultCount=1
    result: one real office record (officeId 1976, 55 Baker Street, W1U 8AN) with no credential presented
    status: 200
  - request: GET https://api-v3.web.prd-knightfrank.com/person?term=smith&isoCode=GB&languageCode=en&maxResultCount=1
    result: one real staff record (empNo, direct dial, mobile, email) with no credential presented
    status: 200
  name: none
  sources:
  - openapi/knight-frank-api-v3-openapi.json
  surface: https://api-v3.web.prd-knightfrank.com
  type: none
- bearerFormat: JWT
  claims_supported:
  - extension_HubContactId
  - oid
  - sub
  - tid
  - iss
  - iat
  - exp
  - aud
  - acr
  - nonce
  - auth_time
  detail: Consumer identity, not developer identity. The Angular front end binds the api-v2 /secure base to an Azure AD B2C scope through an MSAL protectedResourceMap and drives an authorization-code redirect flow. Every anonymous request to /properties/search and /secure/account returns HTTP 401 with a zero-byte body.
  flows:
  - flow: authorizationCode
    id_token_signing_alg:
    - RS256
    response_types:
    - code
    - code id_token
    - code token
    - code id_token token
    - id_token
    - id_token token
    - token
    - token id_token
    subject_types:
    - pairwise
    token_endpoint_auth_methods:
    - client_secret_post
    - client_secret_basic
  name: azure-ad-b2c
  note: The custom claim extension_HubContactId links a B2C consumer account to a contact record in an internal Knight Frank "Hub" CRM.
  openIdConnectUrl: https://login.prd-knightfrank.com/ea15e386-0dbc-4a5b-ac74-08f50f444486/B2C_1A_MYKFSIGNIN/v2.0/.well-known/openid-configuration
  provider:
    b2clogin_domain: knightfrankb2cprod.b2clogin.com
    custom_domain: login.prd-knightfrank.com
    platform: Azure AD B2C
    policy: B2C_1A_MYKFSIGNIN
    tenant_domain: KnightFrankB2Cprod.onmicrosoft.com
    tenant_id: ea15e386-0dbc-4a5b-ac74-08f50f444486
  scheme: bearer
  scopes_detail: scopes/knight-frank-scopes.yml
  sources:
  - authentication/knight-frank-b2c-mykfsignin-openid-configuration.json
  - authentication/knight-frank-b2clogin-mykfsignin-openid-configuration.json
  surface: https://api-v2.web.prd-knightfrank.com
  type: openIdConnect
slug: knight-frank-authentication
source_filename: knight-frank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: >-\n  Live probes of both Knight Frank service hosts on 2026-07-26, the harvested\n  OpenAPI 3.0.1 document at openapi/knight-frank-api-v3-openapi.json, the two\n  harvested Azure AD B2C OpenID Connect discovery documents in this directory,\n  and the public client-side `kfsearchconfig` object plus the MSAL\n  protected-resource map in the site's Angular bundle.\ndescription: >-\n  Knight Frank runs two authentication postures at once and neither is a\n  developer credential. The corporate search service (api-v3) enforces NO\n  authentication at all — its OpenAPI declares no securitySchemes, sends no\n  security requirement, and answers anonymous GETs with real office and\n  people-directory records. The property/account service (api-v2) is fully\n  closed — every request without a bearer token returns 401 — and is protected\n  by Azure AD B2C through a first-party MSAL client belonging to the consumer\n  \"My Knight Frank\"\
  \ saved-property account. There is no API key programme, no\n  client-credentials flow, no developer application registration and no way for\n  a third party to obtain a credential of any kind.\nsummary:\n  types: [none, oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  developer_credential_available: false\nschemes:\n  - name: none\n    type: none\n    surface: https://api-v3.web.prd-knightfrank.com\n    sources: [openapi/knight-frank-api-v3-openapi.json]\n    detail: >-\n      The harvested OpenAPI 3.0.1 document contains no components.securitySchemes\n      block and no security array. Verified live on 2026-07-26: GET /office,\n      GET /office/{id}, GET /person, GET /person/autocomplete, GET /person/cms-search,\n      GET /search, GET /cmspage, GET /intelligencelab and GET /service-lines all\n      returned HTTP 200 with real JSON to a client presenting no credential.\n    evidence:\n      - request: GET https://api-v3.web.prd-knightfrank.com/office?term=london&isoCode=GB&languageCode=en&maxResultCount=1\n\
  \        status: 200\n        result: one real office record (officeId 1976, 55 Baker Street, W1U 8AN) with no credential presented\n      - request: GET https://api-v3.web.prd-knightfrank.com/person?term=smith&isoCode=GB&languageCode=en&maxResultCount=1\n        status: 200\n        result: one real staff record (empNo, direct dial, mobile, email) with no credential presented\n  - name: azure-ad-b2c\n    type: openIdConnect\n    surface: https://api-v2.web.prd-knightfrank.com\n    scheme: bearer\n    bearerFormat: JWT\n    sources:\n      - authentication/knight-frank-b2c-mykfsignin-openid-configuration.json\n      - authentication/knight-frank-b2clogin-mykfsignin-openid-configuration.json\n    openIdConnectUrl: https://login.prd-knightfrank.com/ea15e386-0dbc-4a5b-ac74-08f50f444486/B2C_1A_MYKFSIGNIN/v2.0/.well-known/openid-configuration\n    detail: >-\n      Consumer identity, not developer identity. The Angular front end binds the\n      api-v2 /secure base to an Azure AD B2C scope\
  \ through an MSAL\n      protectedResourceMap and drives an authorization-code redirect flow. Every\n      anonymous request to /properties/search and /secure/account returns HTTP 401\n      with a zero-byte body.\n    provider:\n      platform: Azure AD B2C\n      tenant_domain: KnightFrankB2Cprod.onmicrosoft.com\n      tenant_id: ea15e386-0dbc-4a5b-ac74-08f50f444486\n      custom_domain: login.prd-knightfrank.com\n      b2clogin_domain: knightfrankb2cprod.b2clogin.com\n      policy: B2C_1A_MYKFSIGNIN\n    flows:\n      - flow: authorizationCode\n        response_types: [code, code id_token, code token, code id_token token, id_token, id_token token, token, token id_token]\n        token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\n        id_token_signing_alg: [RS256]\n        subject_types: [pairwise]\n    scopes_detail: scopes/knight-frank-scopes.yml\n    claims_supported: [extension_HubContactId, oid, sub, tid, iss, iat, exp, aud, acr, nonce, auth_time]\n    note:\
  \ >-\n      The custom claim extension_HubContactId links a B2C consumer account to a\n      contact record in an internal Knight Frank \"Hub\" CRM.\ndeveloper_onboarding:\n  self_serve_signup: false\n  application_registration: false\n  api_keys: false\n  sandbox: false\n  terms_for_api_use: false\n  note: >-\n    There is nothing to sign up for. No developer portal, no key issuance, no\n    application registration and no API terms of use exist. The only account\n    signup Knight Frank publishes (https://account.knightfrank.com/) is the\n    consumer \"My Knight Frank\" saved-property account, which grants a B2C token\n    scoped to that consumer's own saved properties and alerts — not API access.\ndocs: null\ndocs_note: Knight Frank publishes no authentication documentation of any kind.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knight-frank/refs/heads/main/authentication/knight-frank-authentication.yml
summary_line: none/oauth2/openIdConnect · 2 schemes
tags:
- Real Estate
- United Kingdom
- Property Listings
- Commercial Real Estate
- Valuation
- Brokerage
- Property Management
- Rentals
- PropTech
- Research
---
