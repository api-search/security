---
api_key_in: []
api_specs:
- filename: natwest-account-transaction-openapi.yml
  format: yaml
  label: NatWest Account and Transaction API
  slug: natwest-account-and-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natwest/refs/heads/main/openapi/natwest-account-transaction-openapi.yml
- filename: natwest-payment-initiation-openapi.yml
  format: yaml
  label: NatWest Payment Initiation API
  slug: natwest-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natwest/refs/heads/main/openapi/natwest-payment-initiation-openapi.yml
- filename: natwest-confirmation-of-funds-openapi.yml
  format: yaml
  label: NatWest Confirmation of Funds API
  slug: natwest-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natwest/refs/heads/main/openapi/natwest-confirmation-of-funds-openapi.yml
auth_types:
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Natwest Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: NatWest Group secures its APIs with oauth2, openIdConnect, and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: NatWest Group
provider_slug: natwest
scheme_count: 2
schemes:
- description: TPP client-credentials flow with the ASPSP (obtain a consent/token before PSU authorisation).
  flow: clientCredentials
  name: TPPOAuth2Security
  sources:
  - openapi/natwest-account-transaction-openapi.yml
  - openapi/natwest-confirmation-of-funds-openapi.yml
  - openapi/natwest-payment-initiation-openapi.yml
  tokenUrl: https://ob.sandbox.natwest.com/token
  type: oauth2
- authorizationUrl: https://api.sandbox.natwest.com/authorize
  description: PSU authorisation-code flow with PSD2 SCA (customer approves the consent/payment).
  flow: authorizationCode
  name: PSUOAuth2Security
  sources:
  - openapi/natwest-account-transaction-openapi.yml
  - openapi/natwest-confirmation-of-funds-openapi.yml
  - openapi/natwest-payment-initiation-openapi.yml
  tokenUrl: https://ob.sandbox.natwest.com/token
  type: oauth2
slug: natwest-authentication
source_filename: natwest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.sandbox.natwest.com/.well-known/openid-configuration\ndocs: https://www.bankofapis.com/documentation/security\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  - mutualTLS\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - refreshToken\n  fapi: true\n  psd2_sca: true\n  standard: FAPI 1.0 Advanced (OBIE Read/Write) with PSD2 strong customer authentication\nprofile:\n  issuer: https://api.sandbox.natwest.com\n  authorization_endpoint: https://api.sandbox.natwest.com/authorize\n  token_endpoint: https://ob.sandbox.natwest.com/token\n  registration_endpoint: https://ob.sandbox.natwest.com/register\n  jwks_uri: https://keystore.openbankingtest.org.uk/0015800000jfwxXAAQ/0015800000jfwxXAAQ.jwks\n  scopes_supported: [openid, payments, accounts, fundsconfirmations, profile]\n  grant_types_supported: [authorization_code, refresh_token, client_credentials]\n  response_types_supported: ['code id_token']\n\
  \  response_modes_supported: [fragment]\n  acr_values_supported: ['urn:openbanking:psd2:ca']\n  token_endpoint_auth_methods_supported: [tls_client_auth, private_key_jwt]\n  id_token_signing_alg_values_supported: [PS256]\n  request_object_signing_alg_values_supported: [PS256]\n  tls_client_certificate_bound_access_tokens: true\n  claims_supported: [aud, exp, iat, iss, acr, openbanking_intent_id, sub]\n  dynamic_client_registration: true\n  certificates: OBIE / eIDAS (OBWAC transport + OBSEAL signing) certificates required\nschemes:\n- name: TPPOAuth2Security\n  type: oauth2\n  flow: clientCredentials\n  description: TPP client-credentials flow with the ASPSP (obtain a consent/token before PSU authorisation).\n  tokenUrl: https://ob.sandbox.natwest.com/token\n  sources:\n  - openapi/natwest-account-transaction-openapi.yml\n  - openapi/natwest-confirmation-of-funds-openapi.yml\n  - openapi/natwest-payment-initiation-openapi.yml\n- name: PSUOAuth2Security\n  type: oauth2\n  flow: authorizationCode\n\
  \  description: PSU authorisation-code flow with PSD2 SCA (customer approves the consent/payment).\n  authorizationUrl: https://api.sandbox.natwest.com/authorize\n  tokenUrl: https://ob.sandbox.natwest.com/token\n  sources:\n  - openapi/natwest-account-transaction-openapi.yml\n  - openapi/natwest-confirmation-of-funds-openapi.yml\n  - openapi/natwest-payment-initiation-openapi.yml\nnotes: |\n  Live-verified against the sandbox OIDC discovery document. Client authentication\n  to the token endpoint is mutual-TLS (tls_client_auth) or private_key_jwt, both\n  PS256. Access tokens are certificate-bound. Every request also carries a detached\n  JWS (x-jws-signature) for message integrity on payment/consent operations, and\n  x-fapi-* headers for FAPI interaction context. Requires dynamic client\n  registration with OBIE/eIDAS certificates.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/natwest/refs/heads/main/authentication/natwest-authentication.yml
summary_line: oauth2/openIdConnect/mutualTLS · 2 schemes
tags:
- Banking
- Open Banking
- Financial Services
- Payments
- PSD2
- FAPI
- Fintech
- Account Information
---
