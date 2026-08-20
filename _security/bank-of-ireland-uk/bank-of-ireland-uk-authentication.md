---
api_key_in: []
api_specs:
- filename: bank-of-ireland-uk-open-data-openapi.json
  format: json
  label: Bank of Ireland (UK) Open Data API
  slug: bank-of-ireland-uk-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-ireland-uk/refs/heads/main/openapi/bank-of-ireland-uk-open-data-openapi.json
- filename: bank-of-ireland-uk-account-info-openapi.yaml
  format: yaml
  label: Bank of Ireland (UK) Account & Transaction Information API
  slug: bank-of-ireland-uk-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-ireland-uk/refs/heads/main/openapi/bank-of-ireland-uk-account-info-openapi.yaml
- filename: bank-of-ireland-uk-payment-initiation-openapi.yaml
  format: yaml
  label: Bank of Ireland (UK) Payment Initiation API
  slug: bank-of-ireland-uk-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-ireland-uk/refs/heads/main/openapi/bank-of-ireland-uk-payment-initiation-openapi.yaml
- filename: bank-of-ireland-uk-confirmation-funds-openapi.yaml
  format: yaml
  label: Bank of Ireland (UK) Confirmation of Funds API
  slug: bank-of-ireland-uk-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-ireland-uk/refs/heads/main/openapi/bank-of-ireland-uk-confirmation-funds-openapi.yaml
auth_types:
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Bank Of Ireland Uk Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Bank of Ireland (UK) secures its APIs with oauth2, openIdConnect, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Bank of Ireland (UK)
provider_slug: bank-of-ireland-uk
scheme_count: 4
schemes:
- description: PSU consent flow requiring PSD2 strong customer authentication (SCA). Hybrid response type code id_token, response_mode fragment, PS256-signed request objects; carries the openbanking_intent_id claim.
  flows:
  - authorizationUrl: https://auth.obapi.bankofireland.com/oauth/as/b365/authorization.oauth2
    flow: authorizationCode
    scopes:
    - openid
    - accounts
    - payments
    - fundsconfirmations
    tokenUrl: https://api.obapi.bankofireland.com/oauth/as/token.oauth2
  name: PSUOAuth2Security
  sources:
  - well-known/bank-of-ireland-uk-openid-configuration.json
  - openapi/bank-of-ireland-uk-account-info-openapi.yaml
  type: oauth2
- description: TPP client-credentials flow with the ASPSP for consent creation and back-channel calls.
  flows:
  - flow: clientCredentials
    scopes:
    - accounts
    - payments
    - fundsconfirmations
    tokenUrl: https://api.obapi.bankofireland.com/oauth/as/token.oauth2
  name: TPPOAuth2Security
  sources:
  - well-known/bank-of-ireland-uk-openid-configuration.json
  - openapi/bank-of-ireland-uk-payment-initiation-openapi.yaml
  type: oauth2
- description: Mutual-TLS client authentication (tls_client_auth) using OBIE/eIDAS transport (OBWAC) certificates; access tokens are certificate-bound. This is the transport-layer client authentication the FAPI host enforces before any OAuth exchange.
  name: mutualTLS
  sources:
  - well-known/bank-of-ireland-uk-openid-configuration.json
  type: mutualTLS
- description: OpenID Connect discovery for the UK ASPSP (FAPI ID 0015800000jfQ9aAAE).
  name: OpenIDConnect
  openIdConnectUrl: https://auth.obapi.bankofireland.com/.well-known/openid-configuration
  sources:
  - well-known/bank-of-ireland-uk-openid-configuration.json
  type: openIdConnect
slug: bank-of-ireland-uk-authentication
source_filename: bank-of-ireland-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: well-known/bank-of-ireland-uk-openid-configuration.json, openapi/bank-of-ireland-uk-account-info-openapi.yaml, openapi/bank-of-ireland-uk-payment-initiation-openapi.yaml, openapi/bank-of-ireland-uk-confirmation-funds-openapi.yaml\ndocs: https://developer.bankofireland.com/\nnote: >-\n  FAPI-grade profile confirmed against the LIVE UK FAPI OpenID discovery document\n  at https://auth.obapi.bankofireland.com/.well-known/openid-configuration\n  (issuer https://auth.obapi.bankofireland.com, OBIE version 3.1). Endpoints,\n  signing algorithms and client-auth method are the real published values, not\n  the OBIE spec's authserver.example placeholders.\nsummary:\n  types: [oauth2, openIdConnect, mutualTLS]\n  oauth2_flows: [authorizationCode, clientCredentials]\n  grant_types_supported: [authorization_code, refresh_token, client_credentials]\n  response_types_supported: [code id_token]\n  token_endpoint_auth_methods: [tls_client_auth]\n\
  \  id_token_signing_alg: [PS256]\n  request_object_signing_alg: [PS256]\n  acr_values: [urn:openbanking:psd2:sca]\n  mtls_bound_tokens: true\n  sca_required: true\nendpoints:\n  issuer: https://auth.obapi.bankofireland.com\n  authorization_endpoint: https://auth.obapi.bankofireland.com/oauth/as/b365/authorization.oauth2\n  token_endpoint: https://api.obapi.bankofireland.com/oauth/as/token.oauth2\n  revocation_endpoint: https://api.obapi.bankofireland.com/oauth/as/revoke_token.oauth2\n  jwks_uri: https://auth.obapi.bankofireland.com/pf/JWKS\n  registration_endpoint: https://api.obapi.bankofireland.com/1/api/open-banking/v3.3/register\nschemes:\n- name: PSUOAuth2Security\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.obapi.bankofireland.com/oauth/as/b365/authorization.oauth2\n    tokenUrl: https://api.obapi.bankofireland.com/oauth/as/token.oauth2\n    scopes: [openid, accounts, payments, fundsconfirmations]\n  description: >-\n    PSU consent flow\
  \ requiring PSD2 strong customer authentication (SCA). Hybrid\n    response type code id_token, response_mode fragment, PS256-signed request\n    objects; carries the openbanking_intent_id claim.\n  sources:\n  - well-known/bank-of-ireland-uk-openid-configuration.json\n  - openapi/bank-of-ireland-uk-account-info-openapi.yaml\n- name: TPPOAuth2Security\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.obapi.bankofireland.com/oauth/as/token.oauth2\n    scopes: [accounts, payments, fundsconfirmations]\n  description: TPP client-credentials flow with the ASPSP for consent creation and back-channel calls.\n  sources:\n  - well-known/bank-of-ireland-uk-openid-configuration.json\n  - openapi/bank-of-ireland-uk-payment-initiation-openapi.yaml\n- name: mutualTLS\n  type: mutualTLS\n  description: >-\n    Mutual-TLS client authentication (tls_client_auth) using OBIE/eIDAS transport\n    (OBWAC) certificates; access tokens are certificate-bound. This is the\n    transport-layer\
  \ client authentication the FAPI host enforces before any OAuth\n    exchange.\n  sources: [well-known/bank-of-ireland-uk-openid-configuration.json]\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.obapi.bankofireland.com/.well-known/openid-configuration\n  description: OpenID Connect discovery for the UK ASPSP (FAPI ID 0015800000jfQ9aAAE).\n  sources: [well-known/bank-of-ireland-uk-openid-configuration.json]\nonboarding: >-\n  TPPs must be enrolled on the FCA/OBIE Open Banking Directory and onboard to the\n  Bank of Ireland (UK) entity separately from Bank of Ireland (ROI). Client\n  applications are registered via OBIE Dynamic Client Registration (DCR) at the\n  registration_endpoint using a signed software statement and OB/eIDAS\n  certificates.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-of-ireland-uk/refs/heads/main/authentication/bank-of-ireland-uk-authentication.yml
summary_line: oauth2/openIdConnect/mutualTLS · 4 schemes
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- CMA9
- United Kingdom
- Payments
- Account Information
- Open Data
- FAPI
- Fintech
---
