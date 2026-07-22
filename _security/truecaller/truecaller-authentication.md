---
api_key_in:
- header
- body
auth_types:
- oauth2
- http bearer
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Truecaller Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode (PKCE S256)
- refreshToken
overview: Truecaller secures its APIs with oauth2, http bearer, and apiKey across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode (PKCE S256) and refreshToken flow(s).
provider_name: Truecaller
provider_slug: truecaller
scheme_count: 5
schemes:
- access_token_ttl_seconds: 3600
  api: truecaller:truecaller-oauth-api
  client_credentials: public client_id only (generated on the developer portal); no client secret in the mobile flow
  flows:
  - authorizationUrl: https://oauth-account-noneu.truecaller.com/v1/auth
    flow: authorizationCode
    pkce: required (S256 code challenge; code_verifier exchanged at the token endpoint)
    revocationUrl: https://oauth-account-noneu.truecaller.com/v1/revoke
    scopes:
    - openid
    - profile
    - phone
    - email
    - address
    - offline_access
    tokenUrl: https://oauth-account-noneu.truecaller.com/v1/token
  - flow: refreshToken
    tokenUrl: https://oauth-account-noneu.truecaller.com/v1/token
  id_token_signing: RS256, per-client JWKS at /.well-known/{clientId}/jwks.json
  name: Truecaller OAuth 2.0 (user verification)
  token_type: Bearer
  type: oauth2
- apis:
  - truecaller:truecaller-oauth-api
  - truecaller:truecaller-web-sdk-profile-api
  detail: GET /v1/userinfo (OAuth API) and GET /v1/default (Web SDK profile host) require Authorization Bearer with the access token issued for the verification request.
  name: Bearer access token (userinfo / profile fetch)
  scheme: bearer
  type: http
- api: truecaller:truecaller-otp-verification-api
  detail: GET /v1/otp/client/installation/phoneNumberDetail/{accessToken} is authenticated with the partner's Client ID sent as the clientId header.
  in: header
  name: clientId header (non-Truecaller user validation)
  parameter: clientId
  type: apiKey
- api: truecaller:truecaller-web-sdk-profile-api
  detail: The truecallersdk:// web_verify deep link carries the app key generated from the developer portal as partnerKey; Truecaller then POSTs the access token to the partner's registered callback URL.
  in: query (deep link parameter)
  name: partnerKey (mobile web deep link)
  parameter: partnerKey
  type: apiKey
- api: truecaller:truecaller-for-business-api
  detail: 'Key ID + Secret API Key are created on the business console (max 5 keys per account) and exchanged at POST /clients/{clientAccountId}/token (X-Public-Access: allow header) for a bearer token. Max 10 tokens per 30 minutes; each token is valid 60 minutes. All Verified Business API calls then use Authorization Bearer.'
  in: body (exchanged for a bearer token)
  name: Truecaller for Business API key exchange
  parameters:
  - key_id
  - api_key
  type: apiKey
slug: truecaller-authentication
source_filename: truecaller-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs:\n- https://docs.truecaller.com/truecaller-sdk/android/latest-oauth-sdk-3.3.0/integration-steps/integrating-with-your-backend/fetching-user-token\n- https://docs.truecaller.com/truecaller-for-business/verified-business-api-documentation/getting-started/authentication\n- https://docs.truecaller.com/truecaller-for-business/verified-business-api-documentation/getting-started/generate-access-token\n- https://oauth-account-noneu.truecaller.com/.well-known/openid-configuration\nsummary:\n  types: [oauth2, http bearer, apiKey]\n  oauth2_flows: [authorizationCode (PKCE S256), refreshToken]\n  api_key_in: [header, body]\nschemes:\n- name: Truecaller OAuth 2.0 (user verification)\n  type: oauth2\n  api: truecaller:truecaller-oauth-api\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth-account-noneu.truecaller.com/v1/auth\n    tokenUrl: https://oauth-account-noneu.truecaller.com/v1/token\n    revocationUrl: https://oauth-account-noneu.truecaller.com/v1/revoke\n\
  \    pkce: required (S256 code challenge; code_verifier exchanged at the token endpoint)\n    scopes: [openid, profile, phone, email, address, offline_access]\n  - flow: refreshToken\n    tokenUrl: https://oauth-account-noneu.truecaller.com/v1/token\n  token_type: Bearer\n  access_token_ttl_seconds: 3600\n  id_token_signing: RS256, per-client JWKS at /.well-known/{clientId}/jwks.json\n  client_credentials: public client_id only (generated on the developer portal); no client secret in the mobile flow\n- name: Bearer access token (userinfo / profile fetch)\n  type: http\n  scheme: bearer\n  apis: [truecaller:truecaller-oauth-api, truecaller:truecaller-web-sdk-profile-api]\n  detail: >-\n    GET /v1/userinfo (OAuth API) and GET /v1/default (Web SDK profile host)\n    require Authorization Bearer with the access token issued for the\n    verification request.\n- name: clientId header (non-Truecaller user validation)\n  type: apiKey\n  in: header\n  parameter: clientId\n  api: truecaller:truecaller-otp-verification-api\n\
  \  detail: >-\n    GET /v1/otp/client/installation/phoneNumberDetail/{accessToken} is\n    authenticated with the partner's Client ID sent as the clientId header.\n- name: partnerKey (mobile web deep link)\n  type: apiKey\n  in: query (deep link parameter)\n  parameter: partnerKey\n  api: truecaller:truecaller-web-sdk-profile-api\n  detail: >-\n    The truecallersdk:// web_verify deep link carries the app key generated\n    from the developer portal as partnerKey; Truecaller then POSTs the access\n    token to the partner's registered callback URL.\n- name: Truecaller for Business API key exchange\n  type: apiKey\n  in: body (exchanged for a bearer token)\n  parameters: [key_id, api_key]\n  api: truecaller:truecaller-for-business-api\n  detail: >-\n    Key ID + Secret API Key are created on the business console (max 5 keys\n    per account) and exchanged at POST /clients/{clientAccountId}/token\n    (X-Public-Access: allow header) for a bearer token. Max 10 tokens per 30\n    minutes;\
  \ each token is valid 60 minutes. All Verified Business API calls\n    then use Authorization Bearer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truecaller/refs/heads/main/authentication/truecaller-authentication.yml
summary_line: oauth2/http bearer/apiKey · 5 schemes
tags:
- Company
- Consumer
- Caller ID
- Phone Verification
- Identity
- OAuth
- Spam Detection
- Communications
- Mobile SDK
---
