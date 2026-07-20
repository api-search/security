---
api_key_in: []
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Datarobot Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- implicit
- refreshToken
overview: DataRobot secures its APIs with http, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, implicit, and refreshToken flow(s).
provider_name: DataRobot
provider_slug: datarobot
scheme_count: 3
schemes:
- description: 'Personal API keys serve as bearer tokens. Send them as `Authorization: Bearer <YOUR_API_TOKEN>` against the REST API base URL for your region (US https://app.datarobot.com/api/v2, EU https://app.eu.datarobot.com/api/v2, JP https://app.jp.datarobot.com/api/v2).'
  name: personalApiKey
  scheme: bearer
  source: docs
  type: http
- authorization_endpoint: https://app.datarobot.com/oauth2/auth
  description: OAuth 2.0 / OIDC via app.datarobot.com authorization server (agent and integration auth).
  device_authorization_endpoint: https://app.datarobot.com/oauth2/device/auth
  grant_types:
  - authorization_code
  - implicit
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  issuer: https://app.datarobot.com
  name: oauth2
  pkce:
  - plain
  - S256
  revocation_endpoint: https://app.datarobot.com/oauth2/revoke
  source: https://app.datarobot.com/.well-known/openid-configuration
  token_endpoint: https://app.datarobot.com/oauth2/token
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  - none
  type: oauth2
- id_token_signing_alg:
  - RS256
  name: openIdConnect
  openIdConnectUrl: https://app.datarobot.com/.well-known/openid-configuration
  source: https://app.datarobot.com/.well-known/openid-configuration
  type: openIdConnect
  userinfo_endpoint: https://app.datarobot.com/userinfo
slug: datarobot-authentication
source_filename: datarobot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.datarobot.com/en/docs/api/dev-learning/api-quickstart.html ; https://app.datarobot.com/.well-known/openid-configuration\ndocs: https://docs.datarobot.com/en/docs/api/dev-learning/api-quickstart.html\nsummary:\n  types: [http, oauth2, openIdConnect]\n  http_scheme: bearer\n  primary: personal-api-key\n  oauth2_flows: [authorizationCode, clientCredentials, deviceCode, implicit, refreshToken]\nschemes:\n  - name: personalApiKey\n    type: http\n    scheme: bearer\n    description: >-\n      Personal API keys serve as bearer tokens. Send them as\n      `Authorization: Bearer <YOUR_API_TOKEN>` against the REST API base URL for\n      your region (US https://app.datarobot.com/api/v2, EU https://app.eu.datarobot.com/api/v2,\n      JP https://app.jp.datarobot.com/api/v2).\n    source: docs\n  - name: oauth2\n    type: oauth2\n    description: OAuth 2.0 / OIDC via app.datarobot.com authorization server (agent and integration\
  \ auth).\n    issuer: https://app.datarobot.com\n    authorization_endpoint: https://app.datarobot.com/oauth2/auth\n    token_endpoint: https://app.datarobot.com/oauth2/token\n    device_authorization_endpoint: https://app.datarobot.com/oauth2/device/auth\n    revocation_endpoint: https://app.datarobot.com/oauth2/revoke\n    grant_types: [authorization_code, implicit, client_credentials, refresh_token, \"urn:ietf:params:oauth:grant-type:device_code\"]\n    token_endpoint_auth_methods: [client_secret_post, client_secret_basic, private_key_jwt, none]\n    pkce: [plain, S256]\n    source: https://app.datarobot.com/.well-known/openid-configuration\n  - name: openIdConnect\n    type: openIdConnect\n    openIdConnectUrl: https://app.datarobot.com/.well-known/openid-configuration\n    userinfo_endpoint: https://app.datarobot.com/userinfo\n    id_token_signing_alg: [RS256]\n    source: https://app.datarobot.com/.well-known/openid-configuration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datarobot/refs/heads/main/authentication/datarobot-authentication.yml
summary_line: http/oauth2/openIdConnect · 3 schemes
tags:
- Company
- Artificial Intelligence
- Machine Learning
- MLOps
- Data Science
- Agentic AI
- Predictive Analytics
- Generative AI
---
