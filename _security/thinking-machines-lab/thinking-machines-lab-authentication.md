---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Thinking Machines Lab Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- refreshToken
overview: Thinking Machines Lab secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, and refreshToken flow(s).
provider_name: Thinking Machines Lab
provider_slug: thinking-machines-lab
scheme_count: 2
schemes:
- id_token_signing_alg: RS256
  issuer: https://auth.thinkingmachines.ai
  jwks_uri: https://auth.thinkingmachines.ai/oauth2/jwks
  name: OpenIDConnect
  openIdConnectUrl: https://auth.thinkingmachines.ai/.well-known/openid-configuration
  sources:
  - well-known/thinking-machines-lab-openid-configuration.json
  type: openIdConnect
  userinfo_endpoint: https://auth.thinkingmachines.ai/oauth2/userinfo
- authorization_endpoint: https://auth.thinkingmachines.ai/oauth2/authorize
  device_authorization_endpoint: https://auth.thinkingmachines.ai/oauth2/device_authorization
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  introspection_endpoint: https://auth.thinkingmachines.ai/oauth2/introspection
  name: OAuth2
  pkce: S256
  sources:
  - well-known/thinking-machines-lab-oauth-authorization-server.json
  token_endpoint: https://auth.thinkingmachines.ai/oauth2/token
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: thinking-machines-lab-authentication
source_filename: thinking-machines-lab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://auth.thinkingmachines.ai/.well-known/openid-configuration + oauth-authorization-server\ndocs: https://tinker-docs.thinkingmachines.ai/\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - deviceCode\n  - refreshToken\n  notes: >-\n    Tinker authenticates through a dedicated OAuth 2.0 / OpenID Connect authorization\n    server at auth.thinkingmachines.ai. The Python SDK obtains and refreshes tokens;\n    the device-code grant supports CLI / headless sign-in and client_credentials\n    supports service (machine-to-machine) access.\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.thinkingmachines.ai/.well-known/openid-configuration\n  issuer: https://auth.thinkingmachines.ai\n  id_token_signing_alg: RS256\n  userinfo_endpoint: https://auth.thinkingmachines.ai/oauth2/userinfo\n  jwks_uri: https://auth.thinkingmachines.ai/oauth2/jwks\n\
  \  sources:\n  - well-known/thinking-machines-lab-openid-configuration.json\n- name: OAuth2\n  type: oauth2\n  authorization_endpoint: https://auth.thinkingmachines.ai/oauth2/authorize\n  token_endpoint: https://auth.thinkingmachines.ai/oauth2/token\n  device_authorization_endpoint: https://auth.thinkingmachines.ai/oauth2/device_authorization\n  introspection_endpoint: https://auth.thinkingmachines.ai/oauth2/introspection\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:device_code'\n  pkce: S256\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_basic\n  - client_secret_post\n  sources:\n  - well-known/thinking-machines-lab-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thinking-machines-lab/refs/heads/main/authentication/thinking-machines-lab-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Ai
- Machine Learning
- LLM
- Fine Tuning
- Model Training
- Developer Tools
- Reinforcement Learning
---
