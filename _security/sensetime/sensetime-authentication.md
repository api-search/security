---
api_key_in: []
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Sensetime Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
- refreshToken
overview: SenseTime secures its APIs with apiKey, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, implicit, and refreshToken flow(s).
provider_name: SenseTime
provider_slug: sensetime
scheme_count: 2
schemes:
- description: Access Key ID + Secret Access Key issued in the SenseNova console. The client library signs a JWT from the key pair and sends it as a Bearer token in the Authorization header. Configured via SENSENOVA_ACCESS_KEY_ID and SENSENOVA_SECRET_ACCESS_KEY environment variables (or sensenova.access_key_id / sensenova.secret_access_key in the Python SDK).
  in: header
  name: SenseNovaAccessKey
  scheme_name: Authorization
  sources:
  - pypi:sensenova
  - docs
  type: apiKey
- authorization_endpoint: https://signin.sensecore.cn/oauth2/auth
  grant_types:
  - authorization_code
  - implicit
  - client_credentials
  - refresh_token
  issuer: https://signin.sensecore.cn/
  jwks_uri: https://signin.sensecore.cn/.well-known/jwks.json
  name: SenseCoreOIDC
  openIdConnectUrl: https://platform.sensenova.cn/.well-known/openid-configuration
  scopes:
  - openid
  - offline
  - offline_access
  sources:
  - well-known/sensetime-openid-configuration.json
  token_endpoint: https://signin.sensecore.cn/oauth2/token
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  - none
  type: openIdConnect
slug: sensetime-authentication
source_filename: sensetime-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://pypi.org/project/sensenova/\ndocs: https://platform.sensenova.cn/en/docs\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_model: access-key-id + secret-access-key (AK/SK)\n  oauth2_flows: [authorizationCode, clientCredentials, implicit, refreshToken]\n  notes: >-\n    The primary SenseNova LLM API auth is an Access Key ID / Secret Access Key pair\n    used to sign a short-lived JWT presented in the Authorization header. OAuth2 /\n    OIDC is available at the SenseCore identity provider (signin.sensecore.cn) as\n    surfaced by the platform's /.well-known/openid-configuration document.\nschemes:\n- name: SenseNovaAccessKey\n  type: apiKey\n  in: header\n  scheme_name: Authorization\n  description: >-\n    Access Key ID + Secret Access Key issued in the SenseNova console. The client\n    library signs a JWT from the key pair and sends it as a Bearer token in the\n    Authorization header. Configured via\
  \ SENSENOVA_ACCESS_KEY_ID and\n    SENSENOVA_SECRET_ACCESS_KEY environment variables (or sensenova.access_key_id /\n    sensenova.secret_access_key in the Python SDK).\n  sources: [pypi:sensenova, docs]\n- name: SenseCoreOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://platform.sensenova.cn/.well-known/openid-configuration\n  issuer: https://signin.sensecore.cn/\n  authorization_endpoint: https://signin.sensecore.cn/oauth2/auth\n  token_endpoint: https://signin.sensecore.cn/oauth2/token\n  jwks_uri: https://signin.sensecore.cn/.well-known/jwks.json\n  grant_types: [authorization_code, implicit, client_credentials, refresh_token]\n  scopes: [openid, offline, offline_access]\n  token_endpoint_auth_methods: [client_secret_post, client_secret_basic, private_key_jwt, none]\n  sources: [well-known/sensetime-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensetime/refs/heads/main/authentication/sensetime-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 2 schemes
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Foundation Models
- Large Language Models
- Generative AI
- Computer Vision
- LLM API
---
