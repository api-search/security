---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Sensely Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sensely declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Sensely
provider_slug: sensely
scheme_count: 5
schemes:
- description: Primary partner authentication. The SDK posts a partner username and password and receives a token, a refresh token and an id token. The same username/password pair is passed to the iOS SDK's SenselyWidget.initialize alongside a procedureId.
  endpoint: POST https://apis.sensely.com/authenticate/authenticate
  in: body
  name: partnerCredentials
  observed_status: 200 (GET to the same path returned HTTP 200, application/json, 740 bytes, 2026-08-26)
  request_fields:
  - username
  - password
  - qa
  scheme: custom
  type: http
- description: Exchanges a refresh token for a new access token. The SDK sends region (observed value "UK") when operating against a non-default regional deployment.
  endpoint: POST https://apis.sensely.com/authenticate/refresh
  name: refreshToken
  request_fields:
  - refresh_token
  - region
  - qa
  scheme: bearer
  type: http
- description: AWS API Gateway key required on the unauthenticated /pub/* endpoints (reset-password, verify-program-code). A key value is embedded in the publicly served Web SDK bundle, so it is a publishable client key rather than a secret; the value is deliberately not recorded in this artifact. Any request to apis.sensely.com without it returns HTTP 403 with x-amzn-errortype ForbiddenException.
  in: header
  name: x-api-key
  type: apiKey
- description: Sensely's member identity is an Amazon Cognito user pool (us-west-1_pMO3JfnoS, region us-west-1). Its OIDC discovery document is publicly readable and was fetched successfully.
  discovery:
    authorization_endpoint: https://cognito-idp.us-west-1.amazonaws.com/us-west-1_pMO3JfnoS/authorize
    end_session_endpoint: https://cognito-idp.us-west-1.amazonaws.com/us-west-1_pMO3JfnoS/logout
    id_token_signing_alg_values_supported:
    - RS256
    issuer: https://cognito-idp.us-west-1.amazonaws.com/us-west-1_pMO3JfnoS
    jwks_uri: https://cognito-idp.us-west-1.amazonaws.com/us-west-1_pMO3JfnoS/.well-known/jwks.json
    response_types_supported:
    - code
    - token
    revocation_endpoint: https://cognito-idp.us-west-1.amazonaws.com/us-west-1_pMO3JfnoS/revoke
    subject_types_supported:
    - public
    token_endpoint: https://cognito-idp.us-west-1.amazonaws.com/us-west-1_pMO3JfnoS/token
    token_endpoint_auth_methods_supported:
    - client_secret_basic
    - client_secret_post
    userinfo_endpoint: https://cognito-idp.us-west-1.amazonaws.com/us-west-1_pMO3JfnoS/userInfo
  name: cognitoOIDC
  openIdConnectUrl: https://cognito-idp.us-west-1.amazonaws.com/us-west-1_pMO3JfnoS/.well-known/openid-configuration
  type: openIdConnect
- description: For the AskFirst (NHS) deployment the widget federates to NHS login via https://nhslogin.sense.ly/Home/NHSLogin?type=web&redirect_url= (a QA host, nhslogin-qa.sense.ly, is also referenced in the bundle). This is a UK-specific citizen identity path, not a partner credential.
  name: nhsLogin
  type: oauth2
slug: sensely-authentication
source_filename: sensely-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  Sensely's published Web SDK bundle (https://clinician-web.sense.ly/latest/sensely.umd.js.min,\n  HTTP 200, 2026-08-26), the iOS SDK README at github.com/Sensely/SenselySDK-iOS, and a live fetch of\n  the OIDC discovery document for the Cognito user pool that bundle names\n  (https://cognito-idp.us-west-1.amazonaws.com/us-west-1_pMO3JfnoS/.well-known/openid-configuration,\n  HTTP 200, 2026-08-26).\napi: sensely-platform-api\nnote: >-\n  Sensely publishes no OpenAPI and no public authentication reference — the SDK READMEs say full\n  documentation is released only to partners under an executed Partner Agreement. Everything below was\n  observed directly: either in the JavaScript Sensely itself serves to every visitor of its demo, or\n  by fetching the identity provider's own discovery document. No credential value is recorded here.\nschemes:\n- name: partnerCredentials\n  type: http\n  scheme: custom\n  in: body\n  endpoint:\
  \ 'POST https://apis.sensely.com/authenticate/authenticate'\n  request_fields: [username, password, qa]\n  description: >-\n    Primary partner authentication. The SDK posts a partner username and password and receives a\n    token, a refresh token and an id token. The same username/password pair is passed to the iOS\n    SDK's SenselyWidget.initialize alongside a procedureId.\n  observed_status: '200 (GET to the same path returned HTTP 200, application/json, 740 bytes, 2026-08-26)'\n- name: refreshToken\n  type: http\n  scheme: bearer\n  endpoint: 'POST https://apis.sensely.com/authenticate/refresh'\n  request_fields: [refresh_token, region, qa]\n  description: >-\n    Exchanges a refresh token for a new access token. The SDK sends region (observed value \"UK\") when\n    operating against a non-default regional deployment.\n- name: apiKey\n  type: apiKey\n  in: header\n  name: x-api-key\n  description: >-\n    AWS API Gateway key required on the unauthenticated /pub/* endpoints (reset-password,\n\
  \    verify-program-code). A key value is embedded in the publicly served Web SDK bundle, so it is a\n    publishable client key rather than a secret; the value is deliberately not recorded in this\n    artifact. Any request to apis.sensely.com without it returns HTTP 403 with\n    x-amzn-errortype ForbiddenException.\n- name: cognitoOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://cognito-idp.us-west-1.amazonaws.com/us-west-1_pMO3JfnoS/.well-known/openid-configuration\n  description: >-\n    Sensely's member identity is an Amazon Cognito user pool (us-west-1_pMO3JfnoS, region us-west-1).\n    Its OIDC discovery document is publicly readable and was fetched successfully.\n  discovery:\n    issuer: https://cognito-idp.us-west-1.amazonaws.com/us-west-1_pMO3JfnoS\n    authorization_endpoint: https://cognito-idp.us-west-1.amazonaws.com/us-west-1_pMO3JfnoS/authorize\n    token_endpoint: https://cognito-idp.us-west-1.amazonaws.com/us-west-1_pMO3JfnoS/token\n    userinfo_endpoint: https://cognito-idp.us-west-1.amazonaws.com/us-west-1_pMO3JfnoS/userInfo\n\
  \    revocation_endpoint: https://cognito-idp.us-west-1.amazonaws.com/us-west-1_pMO3JfnoS/revoke\n    end_session_endpoint: https://cognito-idp.us-west-1.amazonaws.com/us-west-1_pMO3JfnoS/logout\n    jwks_uri: https://cognito-idp.us-west-1.amazonaws.com/us-west-1_pMO3JfnoS/.well-known/jwks.json\n    response_types_supported: [code, token]\n    id_token_signing_alg_values_supported: [RS256]\n    token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n    subject_types_supported: [public]\n- name: nhsLogin\n  type: oauth2\n  description: >-\n    For the AskFirst (NHS) deployment the widget federates to NHS login via\n    https://nhslogin.sense.ly/Home/NHSLogin?type=web&redirect_url= (a QA host,\n    nhslogin-qa.sense.ly, is also referenced in the bundle). This is a UK-specific citizen identity\n    path, not a partner credential.\ngaps:\n- 'No public authentication reference page — the SDK READMEs route to a Google Form request-access flow.'\n- 'No /.well-known/openid-configuration\
  \ or /.well-known/oauth-authorization-server on any Sensely-controlled host.'\n- 'Token lifetime, rotation policy and refresh window are not published.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensely/refs/heads/main/authentication/sensely-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Healthcare
- Digital Health
- Conversational AI
- Virtual Assistant
- Symptom Checker
- Patient Engagement
- Health Insurance
- Mental Health
- SDK
---
