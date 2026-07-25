---
api_key_in: []
api_specs:
- filename: mettle-open-data-api-openapi.json
  format: json
  label: Mettle Open Data Product API
  slug: mettle-open-data-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mettle/refs/heads/main/openapi/mettle-open-data-api-openapi.json
auth_types:
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Mettle Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Mettle secures its APIs with oauth2, openIdConnect, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Mettle
provider_slug: mettle
scheme_count: 3
schemes:
- applies_to:
  - aisp
  - pisp
  - cbpii
  flows:
  - authorizationUrl: https://secure1.natwest.com/as/authorization.oauth2
    flow: authorizationCode
    tokenUrl: https://secure1t.natwest.com/as/token.oauth2
    use: AIS/PIS/CBPII customer-consent access (accounts, payments, fundsconfirmations)
  - flow: clientCredentials
    tokenUrl: https://secure1t.natwest.com/as/token.oauth2
    use: TPP client access-token acquisition prior to consent
  name: OpenBankingOAuth2
  type: oauth2
- acr_values:
  - urn:openbanking:psd2:ca
  - urn:openbanking:psd2:sca
  claims:
  - openbanking_intent_id
  - acr
  - sub
  - iss
  - aud
  - exp
  - iat
  id_token_signing_alg:
  - PS256
  - RS256
  - ES256
  name: OpenIDConnect
  note: FAPI hybrid flow; request object is a signed JWT carrying openbanking_intent_id
  request_object_signing_alg:
  - PS256
  - RS256
  - ES256
  response_types:
  - code id_token
  type: openIdConnect
- name: MutualTLS
  note: OBIE/eIDAS OB Transport certificate for the mTLS channel; OB Signing certificate for detached JWS message signing on write operations.
  token_endpoint_auth_methods:
  - tls_client_auth
  - private_key_jwt
  type: mutualTLS
slug: mettle-authentication
source_filename: mettle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: >-\n  https://secure1.natwest.com/.well-known/openid-configuration (NatWest Group\n  Open Banking OpenID Provider) + OBIE FAPI Read/Write security profile\ndocs: https://www.bankofapis.com/products/accounts/documentation/mettle\nnotes: >-\n  The public Open Data (Product) API is unsecured (no credentials required to read\n  reference data). The Read/Write family (AIS/PIS/CBPII) is FAPI-secured against the\n  shared NatWest Group OpenID Provider. Onboarding requires OBIE/eIDAS OB Transport\n  and Signing certificates issued via the OpenBanking Directory and registration\n  through the Bank of APIs portal.\nsummary:\n  types: [oauth2, openIdConnect, mutualTLS]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  open_data_api: unsecured\n  fapi: true\n  psd2_sca: true\nprovider:\n  issuer: https://secure1.natwest.com\n  authorization_endpoint: https://secure1.natwest.com/as/authorization.oauth2\n\
  \  token_endpoint: https://secure1t.natwest.com/as/token.oauth2\n  revocation_endpoint: https://secure1.natwest.com/as/revoke_token.oauth2\n  registration_endpoint: https://api.natwest.com/register/v1.0\n  jwks_uri: https://keystore.openbanking.org.uk/0015800000jfwxXAAQ/6htRg5BcPIKPQEMSacgHjn.jwks\nschemes:\n- name: OpenBankingOAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure1.natwest.com/as/authorization.oauth2\n    tokenUrl: https://secure1t.natwest.com/as/token.oauth2\n    use: AIS/PIS/CBPII customer-consent access (accounts, payments, fundsconfirmations)\n  - flow: clientCredentials\n    tokenUrl: https://secure1t.natwest.com/as/token.oauth2\n    use: TPP client access-token acquisition prior to consent\n  applies_to: [aisp, pisp, cbpii]\n- name: OpenIDConnect\n  type: openIdConnect\n  response_types: [code id_token]\n  id_token_signing_alg: [PS256, RS256, ES256]\n  request_object_signing_alg: [PS256, RS256, ES256]\n  acr_values: ['urn:openbanking:psd2:ca',\
  \ 'urn:openbanking:psd2:sca']\n  claims: [openbanking_intent_id, acr, sub, iss, aud, exp, iat]\n  note: FAPI hybrid flow; request object is a signed JWT carrying openbanking_intent_id\n- name: MutualTLS\n  type: mutualTLS\n  token_endpoint_auth_methods: [tls_client_auth, private_key_jwt]\n  note: >-\n    OBIE/eIDAS OB Transport certificate for the mTLS channel; OB Signing\n    certificate for detached JWS message signing on write operations.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mettle/refs/heads/main/authentication/mettle-authentication.yml
summary_line: oauth2/openIdConnect/mutualTLS · 3 schemes
tags:
- Financial Services
- Banking
- Business Banking
- Open Banking
- PSD2
- OBIE
- FAPI
- United Kingdom
- Payments
- Account Information
- Challenger Bank
- Fintech
---
