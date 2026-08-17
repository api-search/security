---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Airpr Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: AirPR secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: AirPR
provider_slug: airpr
scheme_count: 2
schemes:
- endpoints:
    authorization: https://crawler-api-auth.onclusive.com/oauth2/authorize
    end_session: https://crawler-api-auth.onclusive.com/logout
    jwks_uri: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_F0XmSWr9T/.well-known/jwks.json
    revocation: https://crawler-api-auth.onclusive.com/oauth2/revoke
    token: https://crawler-api-auth.onclusive.com/oauth2/token
    userinfo: https://crawler-api-auth.onclusive.com/oauth2/userInfo
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_F0XmSWr9T
  name: OnclusiveDeveloperPortalOIDC
  openIdConnectUrl: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_F0XmSWr9T/.well-known/openid-configuration
  response_types_supported:
  - code
  - token
  scopes_supported:
  - openid
  - email
  - phone
  - profile
  sources:
  - well-known/airpr-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
- name: AWS_SigV4
  note: The developer portal ships the standard AWS API Gateway JS SDK (sigV4Client.js + apigClient.js) and a Cognito identity pool (us-east-1:2709e35d-5527-4556-8068-c0c6987bce78), so portal-issued calls are signed with AWS Signature Version 4 using credentials vended by that identity pool. Recorded because the client code is public; the API operations it signs for are not.
  scheme: aws-sigv4
  sources:
  - https://developer.onclusive.com/apigateway-js-sdk/apigClient.js
  type: http
slug: airpr-authentication
source_filename: airpr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_F0XmSWr9T/.well-known/openid-configuration\ndocs: https://developer.onclusive.com/\nnote: >-\n  DERIVED FROM A LIVE, ANONYMOUS OIDC DISCOVERY DOCUMENT — not from an OpenAPI,\n  because Onclusive publishes no OpenAPI. AirPR was absorbed into Onclusive and\n  airpr.com now 301s to onclusive.com, so the surviving developer surface is\n  Onclusive's. https://developer.onclusive.com/ is an AWS API Gateway Developer\n  Portal (the aws-samples serverless reference app) whose /config.js names\n  Amazon Cognito user pool us-east-1_F0XmSWr9T with hosted-UI domain\n  crawler-api-auth.onclusive.com. That user pool's OIDC discovery document is\n  anonymously readable and is the only machine-readable contract-adjacent\n  artifact this company publishes. The API catalog itself is NOT readable: the\n  portal's backing REST API returns 403 \"Missing Authentication Token\" and the\n  portal's\
  \ own content bundle returns 403 AccessDenied from S3.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  identity_provider: Amazon Cognito\n  gated: true\n  gate: >-\n    Registration in the Cognito user pool is required before the developer\n    portal will render an API catalog; no anonymous path to a contract exists.\n\nschemes:\n- name: OnclusiveDeveloperPortalOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_F0XmSWr9T/.well-known/openid-configuration\n  issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_F0XmSWr9T\n  sources:\n  - well-known/airpr-openid-configuration.json\n  endpoints:\n    authorization: https://crawler-api-auth.onclusive.com/oauth2/authorize\n    token: https://crawler-api-auth.onclusive.com/oauth2/token\n    revocation: https://crawler-api-auth.onclusive.com/oauth2/revoke\n    userinfo: https://crawler-api-auth.onclusive.com/oauth2/userInfo\n\
  \    end_session: https://crawler-api-auth.onclusive.com/logout\n    jwks_uri: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_F0XmSWr9T/.well-known/jwks.json\n  response_types_supported:\n  - code\n  - token\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  scopes_supported:\n  - openid\n  - email\n  - phone\n  - profile\n\n- name: AWS_SigV4\n  type: http\n  scheme: aws-sigv4\n  sources:\n  - https://developer.onclusive.com/apigateway-js-sdk/apigClient.js\n  note: >-\n    The developer portal ships the standard AWS API Gateway JS SDK\n    (sigV4Client.js + apigClient.js) and a Cognito identity pool\n    (us-east-1:2709e35d-5527-4556-8068-c0c6987bce78), so portal-issued calls are\n    signed with AWS Signature Version 4 using credentials vended by that\n    identity pool. Recorded because the client code is public; the API\n    operations it signs\
  \ for are not.\n\nx-not-found:\n  api_keys: >-\n    No API key scheme is documented on any public Onclusive page. The Media API\n    product page names no authentication method at all.\n  basic_auth: not documented\n  mutual_tls: not documented\n\nx-evidence:\n- url: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_F0XmSWr9T/.well-known/openid-configuration\n  status: 200\n  content_type: application/json\n- url: https://developer.onclusive.com/config.js\n  status: 200\n  content_type: application/javascript\n- url: https://rcbv8po81k.execute-api.us-east-1.amazonaws.com/prod/catalog\n  status: 403\n  body: '{\"message\":\"Missing Authentication Token\"}'\n- url: https://developer.onclusive.com/custom-content/content-fragments/home/index.md\n  status: 403\n  body: S3 AccessDenied\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airpr/refs/heads/main/authentication/airpr-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Public Relations
- Media Intelligence
- Media Monitoring
- Analytics
- Communications
- Marketing
- PR Measurement
- Onclusive
---
