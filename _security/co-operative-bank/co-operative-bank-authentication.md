---
api_key_in: []
api_specs:
- filename: co-operative-bank-atm-api-openapi.yml
  format: yaml
  label: The Co-operative Bank ATM API
  slug: co-operative-bank-atm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/openapi/co-operative-bank-atm-api-openapi.yml
- filename: co-operative-bank-bca-api-openapi.yml
  format: yaml
  label: The Co-operative Bank BCA API
  slug: co-operative-bank-bca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/openapi/co-operative-bank-bca-api-openapi.yml
- filename: co-operative-bank-branch-api-openapi.yml
  format: yaml
  label: The Co-operative Bank Branch API
  slug: co-operative-bank-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/openapi/co-operative-bank-branch-api-openapi.yml
- filename: co-operative-bank-ccc-api-openapi.yml
  format: yaml
  label: The Co-operative Bank CCC API
  slug: co-operative-bank-ccc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/openapi/co-operative-bank-ccc-api-openapi.yml
- filename: co-operative-bank-pca-api-openapi.yml
  format: yaml
  label: The Co-operative Bank PCA API
  slug: co-operative-bank-pca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/openapi/co-operative-bank-pca-api-openapi.yml
- filename: co-operative-bank-sme-api-openapi.yml
  format: yaml
  label: The Co-operative Bank SME API
  slug: co-operative-bank-sme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/openapi/co-operative-bank-sme-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Co Operative Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: The Co-operative Bank secures its APIs with oauth2, openIdConnect, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: The Co-operative Bank
provider_slug: co-operative-bank
scheme_count: 3
schemes:
- access_token_ttl: 30 minutes
  authorizationUrl: https://bank-retail.apis.co-operativebank.co.uk/apis/oauth/v1/oauth2/auth
  flow: authorizationCode
  grant_types_supported:
  - authorization_code
  - implicit
  - client_credentials
  - refresh_token
  name: OpenBankingOAuth2
  pkce:
    code_challenge_method: S256
    required: true
  refresh_token_ttl: 30 days
  response_types_supported:
  - code
  - code id_token
  - id_token
  - token id_token
  - token
  - token id_token code
  tokenUrl: https://bank-retail.apis.co-operativebank.co.uk/apis/oauth/v1/oauth2/token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  - none
  type: oauth2
- name: OpenIDConnect
  openIdConnectUrl: https://openbanking-retail.apis.co-operativebank.co.uk/apis/oauth/v1/.well-known/openid-configuration
  type: openIdConnect
- description: All API calls require TLS mutual authentication with client transport certificates signed by the Open Banking Directory; certificates must have a minimum of 90 days until expiry (OBWAC/OBSEAL eIDAS certificates).
  name: MutualTLS
  type: mutualTLS
slug: co-operative-bank-authentication
source_filename: co-operative-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: >-\n  https://www.developer.co-operativebank.co.uk/apis/general-specifications/ +\n  https://openbanking-retail.apis.co-operativebank.co.uk/apis/oauth/v1/.well-known/openid-configuration\ndocs: https://www.developer.co-operativebank.co.uk/apis/general-specifications/\nsummary:\n  model: FAPI-grade OAuth2 / OpenID Connect with mutual-TLS and PSD2 SCA (OBIE Read/Write 3.1)\n  types: [oauth2, openIdConnect, mutualTLS]\n  oauth2_flows: [authorizationCode]\n  api_key_in: []\n  transport_security: mutual-TLS (client certificates signed by the Open Banking Directory)\nissuer: https://bank-retail.apis.co-operativebank.co.uk/apis/oauth/v1/\nendpoints:\n  authorization: https://bank-retail.apis.co-operativebank.co.uk/apis/oauth/v1/oauth2/auth\n  token: https://bank-retail.apis.co-operativebank.co.uk/apis/oauth/v1/oauth2/token\n  token_sandbox: https://sandbox-openbanking-retail.apis.co-operativebanktest.co.uk/apis/oauth/v1/oauth2/token\n\
  \  token_production: https://openbanking-retail.apis.co-operativebank.co.uk/apis/oauth/v1/oauth2/token\nschemes:\n- name: OpenBankingOAuth2\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://bank-retail.apis.co-operativebank.co.uk/apis/oauth/v1/oauth2/auth\n  tokenUrl: https://bank-retail.apis.co-operativebank.co.uk/apis/oauth/v1/oauth2/token\n  pkce:\n    required: true\n    code_challenge_method: S256\n  token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic, private_key_jwt, none]\n  grant_types_supported: [authorization_code, implicit, client_credentials, refresh_token]\n  response_types_supported: [code, code id_token, id_token, token id_token, token, token id_token code]\n  access_token_ttl: 30 minutes\n  refresh_token_ttl: 30 days\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://openbanking-retail.apis.co-operativebank.co.uk/apis/oauth/v1/.well-known/openid-configuration\n- name: MutualTLS\n  type: mutualTLS\n\
  \  description: >-\n    All API calls require TLS mutual authentication with client transport\n    certificates signed by the Open Banking Directory; certificates must have a\n    minimum of 90 days until expiry (OBWAC/OBSEAL eIDAS certificates).\nstrong_customer_authentication:\n  standard: PSD2 SCA\n  step_up_2fa: >-\n    Two-factor step-up is required in AIS journeys where sensitive data is\n    requested (transactions over 90 days, standing orders, direct debits, or\n    scheduled payments).\nrequest_signing:\n  standard: OBIE JWS detached signature (JAdES)\n  evidence: >-\n    Payment endpoints return UK.OBIE.Signature.Missing / .Malformed / .Invalid /\n    .MissingClaim / .InvalidClaim errors, confirming JWS request-signature\n    validation on PIS payment orders.\nonboarding:\n  model: manual TPP onboarding\n  contact: tpp.onboarding@co-operativebank.co.uk\n  requires: [FCA or Gibraltar FSC regulation, Open Banking Directory SSA (Software Statement Assertion), OB Directory transport\
  \ + signing certificates]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/authentication/co-operative-bank-authentication.yml
summary_line: oauth2/openIdConnect/mutualTLS · 3 schemes
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Confirmation of Funds
- Fintech
---
