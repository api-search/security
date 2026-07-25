---
api_key_in: []
api_specs:
- filename: obie-opendata-api-standard-openapi.json
  format: json
  label: Virgin Money UK Open Data API
  slug: open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virgin-money-uk/refs/heads/main/openapi/obie-opendata-api-standard-openapi.json
auth_types:
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Virgin Money Uk Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Virgin Money UK secures its APIs with oauth2, openIdConnect, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Virgin Money UK
provider_slug: virgin-money-uk
scheme_count: 3
schemes:
- details:
    acr_values_supported:
    - urn:openbanking:psd2:sca
    authorization_endpoint: https://api.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/oidcapi/oauth2/authorize
    grant_types_supported:
    - authorization_code
    - client_credentials
    id_token_signing_alg_values_supported:
    - PS256
    issuer: https://api.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production
    jwks_uri: https://keystore.openbanking.org.uk/0015800000jf8aKAAQ/0015800000jf8aKAAQ.jwks
    registration_endpoint: https://secureapi.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/register
    request_object_signing_alg_values_supported:
    - PS256
    response_types_supported:
    - code id_token
    - code
    subject_types_supported:
    - pairwise
    token_endpoint: https://secureapi.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/oidcapi/oauth2/token
  name: OpenIDConnect
  openIdConnectUrl: https://api.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/.well-known/openid-configuration
  sources:
  - well-known/virgin-money-uk-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://api.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/oidcapi/oauth2/authorize
    flow: authorizationCode
    note: Used for AIS/PIS/CBPII consent authorisation; combined with an openbanking_intent_id claim and PSD2 strong customer authentication.
    scopes:
    - openid
    - accounts
    - payments
    - fundsconfirmations
    tokenUrl: https://secureapi.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/oidcapi/oauth2/token
  - flow: clientCredentials
    note: TPP client-credentials grant to create consent/resource requests.
    tokenUrl: https://secureapi.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/oidcapi/oauth2/token
  name: OAuth2
  sources:
  - well-known/virgin-money-uk-openid-configuration.json
  type: oauth2
- details:
    note: Mutual-TLS client authentication (tls_client_auth) and certificate-bound access tokens per FAPI. TPPs present OBIE (OBWAC/OBSeal) or eIDAS (QWAC/QSEAL) transport/signing certificates. private_key_jwt also supported.
    tls_client_certificate_bound_access_tokens: true
    token_endpoint_auth_methods_supported:
    - client_secret_basic
    - client_secret_post
    - tls_client_auth
    - private_key_jwt
    - client_secret_jwt
  name: mutualTLS
  sources:
  - well-known/virgin-money-uk-openid-configuration.json
  type: mutualTLS
slug: virgin-money-uk-authentication
source_filename: virgin-money-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: well-known/virgin-money-uk-openid-configuration.json\ndocs: https://developer.virginmoney.com/merged/oidc/\nsummary:\n  types: [oauth2, openIdConnect, mutualTLS]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials]\n  profile: FAPI (Financial-grade API) — UK Open Banking / OBIE Read-Write Standard\n  strong_customer_authentication: true\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://api.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/.well-known/openid-configuration\n  sources: [well-known/virgin-money-uk-openid-configuration.json]\n  details:\n    issuer: https://api.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production\n    authorization_endpoint: https://api.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/oidcapi/oauth2/authorize\n    token_endpoint: https://secureapi.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/oidcapi/oauth2/token\n\
  \    registration_endpoint: https://secureapi.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/register\n    jwks_uri: https://keystore.openbanking.org.uk/0015800000jf8aKAAQ/0015800000jf8aKAAQ.jwks\n    response_types_supported: [code id_token, code]\n    grant_types_supported: [authorization_code, client_credentials]\n    id_token_signing_alg_values_supported: [PS256]\n    request_object_signing_alg_values_supported: [PS256]\n    acr_values_supported: [urn:openbanking:psd2:sca]\n    subject_types_supported: [pairwise]\n- name: OAuth2\n  type: oauth2\n  sources: [well-known/virgin-money-uk-openid-configuration.json]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/oidcapi/oauth2/authorize\n    tokenUrl: https://secureapi.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/oidcapi/oauth2/token\n    scopes: [openid, accounts, payments, fundsconfirmations]\n    note: >-\n      Used for AIS/PIS/CBPII\
  \ consent authorisation; combined with an\n      openbanking_intent_id claim and PSD2 strong customer authentication.\n  - flow: clientCredentials\n    tokenUrl: https://secureapi.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/oidcapi/oauth2/token\n    note: TPP client-credentials grant to create consent/resource requests.\n- name: mutualTLS\n  type: mutualTLS\n  sources: [well-known/virgin-money-uk-openid-configuration.json]\n  details:\n    token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, tls_client_auth, private_key_jwt, client_secret_jwt]\n    tls_client_certificate_bound_access_tokens: true\n    note: >-\n      Mutual-TLS client authentication (tls_client_auth) and certificate-bound\n      access tokens per FAPI. TPPs present OBIE (OBWAC/OBSeal) or eIDAS\n      (QWAC/QSEAL) transport/signing certificates. private_key_jwt also supported.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virgin-money-uk/refs/heads/main/authentication/virgin-money-uk-authentication.yml
summary_line: oauth2/openIdConnect/mutualTLS · 3 schemes
tags:
- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Confirmation of Funds
- FAPI
---
