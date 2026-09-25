---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bancomat-flowpay-api-v1-openapi.yml
  format: yaml
  label: FlowPay API (v1)
  slug: flowpay-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bancomat/refs/heads/main/openapi/bancomat-flowpay-api-v1-openapi.yml
- filename: bancomat-flowpay-api-v2-openapi.yml
  format: yaml
  label: FlowPay API (v2)
  slug: flowpay-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bancomat/refs/heads/main/openapi/bancomat-flowpay-api-v2-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Bancomat Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Bancomat secures its APIs with oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Bancomat
provider_slug: bancomat
scheme_count: 3
schemes:
- description: Autorizzazione oauth ottenuta da terze parti con un authorization flow
  flows:
  - authorizationUrl: https://core.flowpay.it/api/openid/authenticate
    flow: authorizationCode
    scopes: 12
    tokenUrl: https://core.flowpay.it/api/oauth/token
  name: ThirdPartyAuthorizationCode
  sources:
  - openapi/bancomat-flowpay-api-v1-openapi.yml
  type: oauth2
- description: Autorizzazione oauth ottenuta da terze parti con client credential flow
  flows:
  - flow: clientCredentials
    scopes: 14
    tokenUrl: https://core.flowpay.it/api/oauth/token
  name: ThirdPartyClientCredential
  sources:
  - openapi/bancomat-flowpay-api-v1-openapi.yml
  type: oauth2
- description: OAuth2 flow
  flows:
  - authorizationUrl: /openid/authenticate
    flow: authorizationCode
    scopes: 14
    tokenUrl: /oauth/token
  - flow: clientCredentials
    scopes: 15
    tokenUrl: /oauth/token
  name: oAuth2
  sources:
  - openapi/bancomat-flowpay-api-v2-openapi.yml
  type: oauth2
slug: bancomat-authentication
source_filename: bancomat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: openapi/bancomat-flowpay-api-v1-openapi.yml, openapi/bancomat-flowpay-api-v2-openapi.yml; \"Autenticazione\"\n  chapter of the v1 contract (docs.flowpay.it) and https://github.com/FlowPay/client-openapi/blob/main/docs/general.md;\n  live OIDC metadata https://core.flowpay.it/api/openid/.well-known/openid-configuration\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: ThirdPartyAuthorizationCode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://core.flowpay.it/api/openid/authenticate\n    tokenUrl: https://core.flowpay.it/api/oauth/token\n    scopes: 12\n  description: Autorizzazione oauth ottenuta da terze parti con un authorization flow\n  sources:\n  - openapi/bancomat-flowpay-api-v1-openapi.yml\n- name: ThirdPartyClientCredential\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://core.flowpay.it/api/oauth/token\n\
  \    scopes: 14\n  description: Autorizzazione oauth ottenuta da terze parti con client credential flow\n  sources:\n  - openapi/bancomat-flowpay-api-v1-openapi.yml\n- name: oAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /openid/authenticate\n    tokenUrl: /oauth/token\n    scopes: 14\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n    scopes: 15\n  description: OAuth2 flow\n  sources:\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\ndocs: https://docs.flowpay.it/\ndetails:\n  issuer: https://core.flowpay.it/api\n  authorization_endpoint: https://core.flowpay.it/api/openid/authenticate\n  token_endpoint: https://core.flowpay.it/api/oauth/token\n  pushed_authorization_request_endpoint: https://core.flowpay.it/api/oauth/par\n  introspection_endpoint: https://core.flowpay.it/api/openid/token/introspection\n  sandbox_issuer: https://core.sandbox-new.flowpay.it/api/openid\n  client_types:\n  - public (client_id only; SPA/mobile) — must use PKCE\n\
  \  - confidential (client_id + client_secret; server-side)\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  pkce: documented (S256 code_challenge example in the v1 contract); in sandbox all clients are confidential but\n    PKCE can still be exercised\n  pushed_authorization_requests: RFC 9126 PAR endpoint /api/oauth/par — \"in development, already usable in sandbox\";\n    request_uri is single-use and time-limited\n  request_objects: JWT request objects (RFC 9101-style) signed ES256 or PS256, aud = issuer, carry an authorization_details-style\n    consent block; signature not verified in sandbox, required in production\n  token_format: bearer access_token, expires_in 3600 (example), refresh_token issued on authorization_code grant\n  id_token_signing_alg:\n  - ES256\n  consent_model: client_credentials token with scope authorization_intent creates a reconciliation consent, which\n    the user then authorises via the authorization_code flow (AIS consents\
  \ recur for 90 days)\n  multi_tenancy: every v1 resource path is prefixed by the tenantID (UUID) the token was granted for; v2 filters\n    tenant from the token\n  onboarding: register a company account on https://developer.flowpay.it (bank-account ownership + identity check),\n    create an application to obtain client_id/client_secret; sandbox enabled immediately, production third-party\n    access after enablement\n  gated_scheme_surface: BANCOMAT scheme (PagoBancomat / BANCOMAT Pay) integration credentials and specs are issued\n    only to members via https://insight.bancomat.it (OTP login) — no public auth surface\nnote: Profile covers the FlowPay open-banking API (a BANCOMAT company). The BANCOMAT scheme itself exposes no public\n  authentication surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bancomat/refs/heads/main/authentication/bancomat-authentication.yml
summary_line: oauth2 · 3 schemes
tags:
- ATM
- Banking
- Financial Services
- Italy
- Mobile Payments
- Payments
- Debit Cards
- Open Banking
- PSD2
- Account Information
- Payment Initiation
- Invoicing
- pagoPA
---
