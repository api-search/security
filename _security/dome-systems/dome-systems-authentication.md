---
api_key_in:
- header
auth_types:
- oauth2
- openIdConnect
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Dome Systems Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- deviceCode
- refreshToken
overview: Dome Systems secures its APIs with oauth2, openIdConnect, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, deviceCode, and refreshToken flow(s).
provider_name: Dome Systems
provider_slug: dome-systems
scheme_count: 3
schemes:
- description: Machine-to-machine access to the Dome API.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.domesystems.ai/api/v1/auth/token
    token_endpoint_auth: client_secret_basic
  issuer: https://api.domesystems.ai
  jwks_uri: https://api.domesystems.ai/.well-known/jwks.json
  name: PlatformOAuth2
  source: https://api.domesystems.ai/.well-known/oauth-authorization-server
  type: oauth2
- authorization_endpoint: https://login.domesystems.ai/oauth2/authorize
  description: User/operator single sign-on for the Dome console and CLI, fronted by WorkOS.
  device_authorization_endpoint: https://login.domesystems.ai/oauth2/device_authorization
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  id_token_signing_alg:
  - RS256
  introspection_endpoint: https://login.domesystems.ai/oauth2/introspection
  issuer: https://login.domesystems.ai
  jwks_uri: https://login.domesystems.ai/oauth2/jwks
  name: DomeLogin
  source: https://login.domesystems.ai/.well-known/openid-configuration
  token_endpoint: https://login.domesystems.ai/oauth2/token
  type: openIdConnect
  userinfo_endpoint: https://login.domesystems.ai/oauth2/userinfo
- description: Per-agent API keys issued at registration (the credential root of trust). The CLI issues and rotates agent API keys; these authenticate an agent's calls through the Gateway and Broker.
  in: header
  name: AgentAPIKey
  source: https://www.domesystems.ai/llms.txt
  type: apiKey
slug: dome-systems-authentication
source_filename: dome-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  https://api.domesystems.ai/.well-known/oauth-authorization-server +\n  https://login.domesystems.ai/.well-known/openid-configuration +\n  https://www.domesystems.ai/llms.txt\nsummary:\n  types: [oauth2, openIdConnect, apiKey]\n  oauth2_flows: [clientCredentials, authorizationCode, deviceCode, refreshToken]\n  api_key_in: [header]\nschemes:\n- name: PlatformOAuth2\n  type: oauth2\n  description: Machine-to-machine access to the Dome API.\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.domesystems.ai/api/v1/auth/token\n    token_endpoint_auth: client_secret_basic\n  issuer: https://api.domesystems.ai\n  jwks_uri: https://api.domesystems.ai/.well-known/jwks.json\n  source: https://api.domesystems.ai/.well-known/oauth-authorization-server\n- name: DomeLogin\n  type: openIdConnect\n  description: User/operator single sign-on for the Dome console and CLI, fronted by WorkOS.\n  issuer: https://login.domesystems.ai\n\
  \  authorization_endpoint: https://login.domesystems.ai/oauth2/authorize\n  token_endpoint: https://login.domesystems.ai/oauth2/token\n  device_authorization_endpoint: https://login.domesystems.ai/oauth2/device_authorization\n  userinfo_endpoint: https://login.domesystems.ai/oauth2/userinfo\n  introspection_endpoint: https://login.domesystems.ai/oauth2/introspection\n  jwks_uri: https://login.domesystems.ai/oauth2/jwks\n  grant_types: [authorization_code, client_credentials, refresh_token, 'urn:ietf:params:oauth:grant-type:device_code']\n  id_token_signing_alg: [RS256]\n  source: https://login.domesystems.ai/.well-known/openid-configuration\n- name: AgentAPIKey\n  type: apiKey\n  in: header\n  description: >-\n    Per-agent API keys issued at registration (the credential root of trust). The CLI\n    issues and rotates agent API keys; these authenticate an agent's calls through the\n    Gateway and Broker.\n  source: https://www.domesystems.ai/llms.txt\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dome-systems/refs/heads/main/authentication/dome-systems-authentication.yml
summary_line: oauth2/openIdConnect/apiKey · 3 schemes
tags:
- Company
- AI Agents
- Agent Governance
- AI Operations
- Authorization
- Audit
- MCP
- Enterprise
- Cedar Policy
- LLM
---
