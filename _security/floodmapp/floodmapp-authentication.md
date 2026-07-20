---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Floodmapp Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: FloodMapp secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: FloodMapp
provider_slug: floodmapp
scheme_count: 1
schemes:
- evidence:
  - observed_client_id: 2a03sn0qcnvtcod1jvvgah7535
  - observed_response_type: code
  - observed_scope: openid
  - redirect_uri: https://api.floodmapp.com/oauth2/idpresponse
  flows:
  - authorizationUrl: https://login.floodmapp.com/oauth2/authorize
    flow: authorizationCode
    scopes:
      openid: OpenID Connect authentication
    tokenUrl: https://login.floodmapp.com/oauth2/token
  name: cognitoOAuth2
  provider: AWS Cognito
  type: oauth2
slug: floodmapp-authentication
source_filename: floodmapp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  Observed live 302 redirect from https://api.floodmapp.com to the AWS Cognito\n  hosted-UI OAuth2 authorization endpoint (login.floodmapp.com/oauth2/authorize).\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  provider: AWS Cognito (login.floodmapp.com)\nnotes: >-\n  FloodMapp's authenticated API surface at api.floodmapp.com is protected by an\n  AWS Cognito user pool. Unauthenticated requests are redirected to the Cognito\n  hosted UI to complete an OAuth2 authorization-code flow. The 'openid' scope in\n  the observed request indicates OpenID Connect. Customer API credentials are\n  provisioned per the FAQ (\"user credentials providing access within hours\");\n  there is no public self-service developer portal. Token and JWKS endpoints\n  follow AWS Cognito conventions for the login.floodmapp.com domain.\nschemes:\n  - name: cognitoOAuth2\n    type: oauth2\n    provider: AWS Cognito\n\
  \    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.floodmapp.com/oauth2/authorize\n        tokenUrl: https://login.floodmapp.com/oauth2/token\n        scopes:\n          openid: OpenID Connect authentication\n    evidence:\n      - observed_client_id: 2a03sn0qcnvtcod1jvvgah7535\n      - observed_response_type: code\n      - observed_scope: openid\n      - redirect_uri: https://api.floodmapp.com/oauth2/idpresponse\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/floodmapp/refs/heads/main/authentication/floodmapp-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Flood Intelligence
- Flood Forecasting
- Geospatial
- GIS
- Emergency Management
- Climate Risk
- Machine Learning
- Hydrology
---
