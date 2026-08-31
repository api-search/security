---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Abm Industries Authentication
name_suffix: Authentication
oauth_flows: []
overview: ABM Industries declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: ABM Industries
provider_slug: abm-industries
scheme_count: 3
schemes:
- authority: https://connect2ABM.b2clogin.com/connect2ABM.onmicrosoft.com/B2C_1_cft-signin
  authorization_endpoint: https://connect2abm.b2clogin.com/connect2abm.onmicrosoft.com/b2c_1_cft-signin/oauth2/v2.0/authorize
  claims:
  - name
  - given_name
  - family_name
  - idp
  - emails
  - sub
  - tfp
  - isForgotPassword
  - iss
  - iat
  - exp
  - aud
  - acr
  - nonce
  - auth_time
  description: Customer sign-in to ABM Connect. Microsoft Authentication Library (MSAL) redirect flow against ABM's Azure AD B2C tenant, user flow B2C_1_cft-signin.
  discovery: https://connect2abm.b2clogin.com/connect2abm.onmicrosoft.com/B2C_1_cft-signin/v2.0/.well-known/openid-configuration
  end_session_endpoint: https://connect2abm.b2clogin.com/connect2abm.onmicrosoft.com/b2c_1_cft-signin/oauth2/v2.0/logout
  flow: authorization_code
  id: azure_ad_b2c_oauth2
  id_token_signing_alg: RS256
  issuer: https://connect2abm.b2clogin.com/01698e86-a3b5-4f25-a6a5-a91df3c194cd/v2.0/
  jwks_uri: https://connect2abm.b2clogin.com/connect2abm.onmicrosoft.com/b2c_1_cft-signin/discovery/v2.0/keys
  pkce: unstated
  scopes:
  - https://connect2ABM.onmicrosoft.com/31f16065-3479-4b3c-a3cd-e337cafc33c9/cft_client_access
  - openid
  subject_type: pairwise
  token_endpoint: https://connect2abm.b2clogin.com/connect2abm.onmicrosoft.com/b2c_1_cft-signin/oauth2/v2.0/token
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  type: oauth2
  verified: probed
- authority: https://login.microsoftonline.com/01698e86-a3b5-4f25-a6a5-a91df3c194cd
  description: A second MSAL configuration in the same bundle targets ABM's corporate Microsoft Entra ID tenant directly (login.microsoftonline.com/<tenant>), used for the internal/employee variant of the app. Same access scope.
  discovery: https://login.microsoftonline.com/01698e86-a3b5-4f25-a6a5-a91df3c194cd/v2.0/.well-known/openid-configuration
  flow: authorization_code
  id: entra_id_oauth2
  type: oauth2
  verified: probed
- description: Azure API Management gateway key. Every unauthenticated request to https://abm-apim.azure-api.net/ returns HTTP 401 with the body "Access denied due to missing subscription key. Make sure to include subscription key when making requests to an API." The connectapi.abm.com gateway answers 404/500 JSON rather than 401, but is the same APIM product.
  evidence:
  - status: 401
    url: https://abm-apim.azure-api.net/
  id: apim_subscription_key
  in: header
  name: Ocp-Apim-Subscription-Key
  type: apiKey
  verified: probed
slug: abm-industries-authentication
source_filename: abm-industries-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: >-\n  ABM's own production client configuration read from https://connect.abm.com/chunk-QN7SXVIA.js\n  and https://connect.abm.com/main-FEOQKLI7.js, plus a live unauthenticated fetch of the resulting\n  Azure AD B2C OpenID Connect discovery document, 2026-08-29.\nprovider: ABM Industries\nproviderId: abm-industries\napi: ABM Connect\nsummary: >-\n  The ABM Connect API is not publicly documented, but its authentication model is fully\n  determinable from the first-party client ABM ships at connect.abm.com. Two layers gate it:\n  an Azure API Management subscription key at the gateway, and an OAuth 2.0 / OpenID Connect\n  bearer token issued by ABM's own Azure AD B2C tenant. There is no self-service signup, no\n  public client registration, and no documented API-key issuance path — credentials come with\n  a facilities-services contract.\nschemes:\n  - id: azure_ad_b2c_oauth2\n    type: oauth2\n    flow: authorization_code\n  \
  \  pkce: unstated\n    description: >-\n      Customer sign-in to ABM Connect. Microsoft Authentication Library (MSAL) redirect flow\n      against ABM's Azure AD B2C tenant, user flow B2C_1_cft-signin.\n    authority: https://connect2ABM.b2clogin.com/connect2ABM.onmicrosoft.com/B2C_1_cft-signin\n    discovery: https://connect2abm.b2clogin.com/connect2abm.onmicrosoft.com/B2C_1_cft-signin/v2.0/.well-known/openid-configuration\n    authorization_endpoint: https://connect2abm.b2clogin.com/connect2abm.onmicrosoft.com/b2c_1_cft-signin/oauth2/v2.0/authorize\n    token_endpoint: https://connect2abm.b2clogin.com/connect2abm.onmicrosoft.com/b2c_1_cft-signin/oauth2/v2.0/token\n    end_session_endpoint: https://connect2abm.b2clogin.com/connect2abm.onmicrosoft.com/b2c_1_cft-signin/oauth2/v2.0/logout\n    jwks_uri: https://connect2abm.b2clogin.com/connect2abm.onmicrosoft.com/b2c_1_cft-signin/discovery/v2.0/keys\n    issuer: https://connect2abm.b2clogin.com/01698e86-a3b5-4f25-a6a5-a91df3c194cd/v2.0/\n\
  \    id_token_signing_alg: RS256\n    subject_type: pairwise\n    token_endpoint_auth_methods:\n      - client_secret_post\n      - client_secret_basic\n    scopes:\n      - https://connect2ABM.onmicrosoft.com/31f16065-3479-4b3c-a3cd-e337cafc33c9/cft_client_access\n      - openid\n    claims:\n      [name, given_name, family_name, idp, emails, sub, tfp, isForgotPassword, iss, iat, exp, aud, acr, nonce, auth_time]\n    verified: probed\n  - id: entra_id_oauth2\n    type: oauth2\n    flow: authorization_code\n    description: >-\n      A second MSAL configuration in the same bundle targets ABM's corporate Microsoft Entra ID\n      tenant directly (login.microsoftonline.com/<tenant>), used for the internal/employee\n      variant of the app. Same access scope.\n    authority: https://login.microsoftonline.com/01698e86-a3b5-4f25-a6a5-a91df3c194cd\n    discovery: https://login.microsoftonline.com/01698e86-a3b5-4f25-a6a5-a91df3c194cd/v2.0/.well-known/openid-configuration\n    verified: probed\n\
  \  - id: apim_subscription_key\n    type: apiKey\n    in: header\n    name: Ocp-Apim-Subscription-Key\n    description: >-\n      Azure API Management gateway key. Every unauthenticated request to\n      https://abm-apim.azure-api.net/ returns HTTP 401 with the body\n      \"Access denied due to missing subscription key. Make sure to include subscription key when\n      making requests to an API.\" The connectapi.abm.com gateway answers 404/500 JSON rather than\n      401, but is the same APIM product.\n    verified: probed\n    evidence:\n      - url: https://abm-apim.azure-api.net/\n        status: 401\nonboarding:\n  self_service: false\n  public_signup: false\n  dynamic_client_registration: false\n  note: >-\n    No developer portal, no key-request form and no published client-registration endpoint were\n    found. Access to ABM Connect is provisioned by ABM to contracted customers.\nhosts:\n  - host: connectapi.abm.com\n    role: customer API gateway (Azure API Management)\n  - host:\
  \ appservices.abm.com\n    role: task-management / ops API host (502 at probe time)\n  - host: abm-apim.azure-api.net\n    role: Azure API Management instance (mock services base)\nevidence:\n  - url: https://connect2abm.b2clogin.com/connect2abm.onmicrosoft.com/B2C_1_cft-signin/v2.0/.well-known/openid-configuration\n    status: 200\n  - url: https://login.microsoftonline.com/01698e86-a3b5-4f25-a6a5-a91df3c194cd/v2.0/.well-known/openid-configuration\n    status: 200\n  - url: https://abm-apim.azure-api.net/\n    status: 401\n  - url: https://connectapi.abm.com/cust-api/\n    status: 500\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abm-industries/refs/heads/main/authentication/abm-industries-authentication.yml
summary_line: 3 schemes
tags:
- Facilities Management
- Engineering
- Infrastructure
- Mobility
- Fortune 500
---
