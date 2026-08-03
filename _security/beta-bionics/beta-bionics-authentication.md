---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Beta Bionics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Beta Bionics secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Beta Bionics
provider_slug: beta-bionics
scheme_count: 2
schemes:
- id_token_signing_alg_values_supported:
  - RS256
  issuer: https://cognito-idp.us-east-2.amazonaws.com/us-east-2_HNbbVuwO8
  jwks_uri: https://cognito-idp.us-east-2.amazonaws.com/us-east-2_HNbbVuwO8/.well-known/jwks.json
  name: CognitoUserPool
  openIdConnectUrl: https://cognito-idp.us-east-2.amazonaws.com/us-east-2_HNbbVuwO8/.well-known/openid-configuration
  provider: Amazon Cognito
  region: us-east-2
  sources:
  - well-known/beta-bionics-openid-configuration.json
  subject_types_supported:
  - public
  type: openIdConnect
  user_pool_id: us-east-2_HNbbVuwO8
- end_session_endpoint: https://us-east-2hnbbvuwo8.auth.us-east-2.amazoncognito.com/logout
  flows:
  - authorizationUrl: https://us-east-2hnbbvuwo8.auth.us-east-2.amazoncognito.com/oauth2/authorize
    flow: authorizationCode
    scopes:
    - openid
    - email
    - phone
    - profile
    tokenUrl: https://us-east-2hnbbvuwo8.auth.us-east-2.amazoncognito.com/oauth2/token
  - authorizationUrl: https://us-east-2hnbbvuwo8.auth.us-east-2.amazoncognito.com/oauth2/authorize
    flow: implicit
    scopes:
    - openid
    - email
    - phone
    - profile
  name: CognitoHostedUI
  response_types_supported:
  - code
  - token
  revocation_endpoint: https://us-east-2hnbbvuwo8.auth.us-east-2.amazoncognito.com/oauth2/revoke
  sources:
  - well-known/beta-bionics-openid-configuration.json
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: oauth2
  userinfo_endpoint: https://us-east-2hnbbvuwo8.auth.us-east-2.amazoncognito.com/oauth2/userInfo
slug: beta-bionics-authentication
source_filename: beta-bionics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://cognito-idp.us-east-2.amazonaws.com/us-east-2_HNbbVuwO8/.well-known/openid-configuration\nnote: >-\n  Derived from a live OIDC discovery fetch, not from an OpenAPI document — Beta\n  Bionics publishes no OpenAPI/Swagger and no developer authentication guide. The\n  Bionic Portal and the iLet / Bionic Circle mobile apps authenticate against an\n  Amazon Cognito user pool via AWS Amplify Auth; the resulting Cognito JWT is\n  presented to the Amazon API Gateway deployment at us-main-prod.betabionicsapi.com.\n  There is no self-service developer registration, no API keys, and no documented\n  third-party access path. Access is provisioned to patients, caregivers (Bionic\n  Circle followers) and clinic staff through the product, and is subject to HIPAA.\nsummary:\n  types: [openIdConnect, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, implicit]\n  public_developer_signup: false\n  human_in_the_loop: true\n\
  schemes:\n- name: CognitoUserPool\n  type: openIdConnect\n  openIdConnectUrl: https://cognito-idp.us-east-2.amazonaws.com/us-east-2_HNbbVuwO8/.well-known/openid-configuration\n  issuer: https://cognito-idp.us-east-2.amazonaws.com/us-east-2_HNbbVuwO8\n  provider: Amazon Cognito\n  user_pool_id: us-east-2_HNbbVuwO8\n  region: us-east-2\n  jwks_uri: https://cognito-idp.us-east-2.amazonaws.com/us-east-2_HNbbVuwO8/.well-known/jwks.json\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  sources: [well-known/beta-bionics-openid-configuration.json]\n- name: CognitoHostedUI\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://us-east-2hnbbvuwo8.auth.us-east-2.amazoncognito.com/oauth2/authorize\n    tokenUrl: https://us-east-2hnbbvuwo8.auth.us-east-2.amazoncognito.com/oauth2/token\n    scopes: [openid, email, phone, profile]\n  - flow: implicit\n    authorizationUrl: https://us-east-2hnbbvuwo8.auth.us-east-2.amazoncognito.com/oauth2/authorize\n\
  \    scopes: [openid, email, phone, profile]\n  revocation_endpoint: https://us-east-2hnbbvuwo8.auth.us-east-2.amazoncognito.com/oauth2/revoke\n  userinfo_endpoint: https://us-east-2hnbbvuwo8.auth.us-east-2.amazoncognito.com/oauth2/userInfo\n  end_session_endpoint: https://us-east-2hnbbvuwo8.auth.us-east-2.amazoncognito.com/logout\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n  response_types_supported: [code, token]\n  sources: [well-known/beta-bionics-openid-configuration.json]\nmfa:\n  supported: true\n  evidence: >-\n    The Bionic Portal client exposes account MFA controls\n    (/v1/account/checkAccountSecurity, /v1/account/toggleMfa) and the Amplify\n    Cognito config carries an mfa block.\n  source: https://portal.betabionics.com/main-QC35MYJM.js\nx-evidence:\n- {fetched: '2026-08-02', url: 'https://cognito-idp.us-east-2.amazonaws.com/us-east-2_HNbbVuwO8/.well-known/openid-configuration', http_status: 200, content_type: application/json}\n\
  - {fetched: '2026-08-02', url: 'https://cognito-idp.us-east-2.amazonaws.com/us-east-2_HNbbVuwO8/.well-known/jwks.json', http_status: 200}\n- {fetched: '2026-08-02', url: 'https://us-main-prod.betabionicsapi.com/', http_status: 403, body: '{\"message\":\"Missing Authentication Token\"}'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beta-bionics/refs/heads/main/authentication/beta-bionics-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Health
- Healthcare
- Medical Devices
- Diabetes
- Automated Insulin Delivery
- Digital Health
- Remote Patient Monitoring
- HIPAA
- Connected Devices
---
