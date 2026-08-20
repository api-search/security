---
api_key_in: []
api_specs:
- filename: yorkshire-building-society-account-information-api-openapi.yaml
  format: yaml
  label: Yorkshire Building Society Account Information API
  slug: ybs-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yorkshire-building-society/refs/heads/main/openapi/yorkshire-building-society-account-information-api-openapi.yaml
- filename: yorkshire-building-society-payment-initiation-api-openapi.yaml
  format: yaml
  label: Yorkshire Building Society Payment Initiation API
  slug: ybs-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yorkshire-building-society/refs/heads/main/openapi/yorkshire-building-society-payment-initiation-api-openapi.yaml
- filename: yorkshire-building-society-confirmation-of-funds-api-openapi.yaml
  format: yaml
  label: Yorkshire Building Society Confirmation of Funds API
  slug: ybs-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yorkshire-building-society/refs/heads/main/openapi/yorkshire-building-society-confirmation-of-funds-api-openapi.yaml
- filename: yorkshire-building-society-event-subscriptions-api-openapi.yaml
  format: yaml
  label: Yorkshire Building Society Event Subscriptions API
  slug: ybs-event-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yorkshire-building-society/refs/heads/main/openapi/yorkshire-building-society-event-subscriptions-api-openapi.yaml
auth_types:
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Yorkshire Building Society Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Yorkshire Building Society secures its APIs with oauth2 and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Yorkshire Building Society
provider_slug: yorkshire-building-society
scheme_count: 3
schemes:
- authorizationUrl: https://authorisation.ybs.co.uk/public/authentication/pre_login.do
  description: PSU-present SCA flow; response_types code / code id_token.
  flow: authorizationCode
  name: PSUOAuth2Security
  scopes:
  - openid
  - accounts
  - payments
  - fundsconfirmations
  sources:
  - openapi/yorkshire-building-society-account-information-api-openapi.yaml
  - openapi/yorkshire-building-society-confirmation-of-funds-api-openapi.yaml
  - openapi/yorkshire-building-society-payment-initiation-api-openapi.yaml
  tokenUrl: https://ob-ybs.api.ybs.co.uk/identity/open-banking/v3.1/token
  type: oauth2
- description: TPP client-credentials flow for consent setup and non-PSU resources.
  flow: clientCredentials
  name: TPPOAuth2Security
  scopes:
  - accounts
  - payments
  - fundsconfirmations
  sources:
  - openapi/yorkshire-building-society-account-information-api-openapi.yaml
  - openapi/yorkshire-building-society-confirmation-of-funds-api-openapi.yaml
  - openapi/yorkshire-building-society-event-subscriptions-api-openapi.yaml
  - openapi/yorkshire-building-society-payment-initiation-api-openapi.yaml
  tokenUrl: https://ob-ybs.api.ybs.co.uk/identity/open-banking/v3.1/token
  type: oauth2
- description: OB/eIDAS transport certificate required on every TLS connection; access tokens are certificate-bound (RFC 8705). Not expressible as an OpenAPI 3.0.1 securityScheme but mandated by the OBIE profile.
  name: MutualTLS
  sources:
  - well-known/yorkshire-building-society-ybs-openid-configuration.json
  type: mutualTLS
slug: yorkshire-building-society-authentication
source_filename: yorkshire-building-society-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: openapi/*-openapi.yaml\ndocs: https://api.ybs.co.uk/open-banking/v1.0/.well-known/ybs/openid-configuration\nnote: >-\n  FAPI-grade OBIE security profile, confirmed against the live OpenID Provider\n  discovery documents (well-known/*-openid-configuration.json). Beyond the two\n  OpenAPI oauth2 schemes, the real deployment layers mutual-TLS transport\n  authentication (certificate-bound access tokens), private_key_jwt client\n  authentication, PS256-signed request objects and detached JWS response\n  signatures (x-jws-signature), and PSD2 strong customer authentication for the\n  PSU-present authorization-code flow.\nsummary:\n  types: [oauth2, mutualTLS]\n  oauth2_flows: [authorizationCode, clientCredentials]\n  token_endpoint_auth_methods: [client_secret_basic, private_key_jwt]\n  request_object_signing_alg: [PS256]\n  id_token_signing_alg: [PS256]\n  mtls_bound_tokens: true\n  sca_required: true\n  profile: FAPI 1.0 / OBIE\
  \ Read-Write Security Profile\nschemes:\n- name: PSUOAuth2Security\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://authorisation.ybs.co.uk/public/authentication/pre_login.do\n  tokenUrl: https://ob-ybs.api.ybs.co.uk/identity/open-banking/v3.1/token\n  scopes: [openid, accounts, payments, fundsconfirmations]\n  description: PSU-present SCA flow; response_types code / code id_token.\n  sources:\n  - openapi/yorkshire-building-society-account-information-api-openapi.yaml\n  - openapi/yorkshire-building-society-confirmation-of-funds-api-openapi.yaml\n  - openapi/yorkshire-building-society-payment-initiation-api-openapi.yaml\n- name: TPPOAuth2Security\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://ob-ybs.api.ybs.co.uk/identity/open-banking/v3.1/token\n  scopes: [accounts, payments, fundsconfirmations]\n  description: TPP client-credentials flow for consent setup and non-PSU resources.\n  sources:\n  - openapi/yorkshire-building-society-account-information-api-openapi.yaml\n\
  \  - openapi/yorkshire-building-society-confirmation-of-funds-api-openapi.yaml\n  - openapi/yorkshire-building-society-event-subscriptions-api-openapi.yaml\n  - openapi/yorkshire-building-society-payment-initiation-api-openapi.yaml\n- name: MutualTLS\n  type: mutualTLS\n  description: >-\n    OB/eIDAS transport certificate required on every TLS connection; access\n    tokens are certificate-bound (RFC 8705). Not expressible as an OpenAPI 3.0.1\n    securityScheme but mandated by the OBIE profile.\n  sources: [well-known/yorkshire-building-society-ybs-openid-configuration.json]\nsigning:\n  request_object_signing_alg: PS256\n  detached_jws_header: x-jws-signature\n  jwks_uri: https://keystore.openbanking.org.uk/0015800001041RIAAY/UXIIubFcTJTeZJHCsEpt0L.jwks\nfapi_headers:\n- x-fapi-interaction-id\n- x-fapi-auth-date\n- x-fapi-customer-ip-address\n- x-customer-user-agent\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yorkshire-building-society/refs/heads/main/authentication/yorkshire-building-society-authentication.yml
summary_line: oauth2/mutualTLS · 3 schemes
tags:
- Financial-Services
- Banking
- Building Society
- Open Banking
- PSD2
- OBIE
- FAPI
- United Kingdom
- Payments
- Account Information
- Fintech
---
