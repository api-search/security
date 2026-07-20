---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Kensho Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Kensho secures its APIs with http and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Kensho
provider_slug: kensho
scheme_count: 4
schemes:
- applies_to:
  - scribe.kensho.com
  - extract.kensho.com
  - nerd.kensho.com
  - kfinance.kensho.com
  description: Bearer access token in the Authorization header for all product APIs.
  name: BearerAuth
  scheme: bearer
  type: http
- description: Development-time personal token issued from the Kensho services platform.
  docs: https://docs.kensho.com/authentication/personal-token
  name: PersonalToken
  scheme: bearer
  type: http
- description: Production authentication using a client ID and private key pair that is exchanged for a short-lived bearer access token.
  docs: https://docs.kensho.com/authentication/keypair
  name: KeyPair
  scheme: bearer
  type: http
- description: OAuth 2.0 for the LLM-ready API hosted MCP server.
  flows:
  - authorizationUrl: https://kfinance.kensho.com/integrations/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://kfinance.kensho.com/integrations/register
    tokenUrl: https://kfinance.kensho.com/integrations/token
  - flow: clientCredentials
    tokenUrl: https://kfinance.kensho.com/integrations/token
  - flow: refreshToken
    tokenUrl: https://kfinance.kensho.com/integrations/token
  issuer: https://kfinance.kensho.com/integrations
  name: OAuth2
  sources:
  - well-known/kensho-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: kensho-authentication
source_filename: kensho-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.kensho.com/authentication\ndocs: https://docs.kensho.com/authentication\nsummary:\n  types: [http, oauth2]\n  http_scheme: bearer\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\nnotes: >-\n  All Kensho product APIs (Scribe, Extract, NERD) authenticate with a bearer\n  access token in the Authorization header. Tokens are issued from the Kensho\n  services platform two ways: a personal token (Authentication Quickstart, for\n  development) and a production key pair (client ID + private key). The\n  LLM-ready API MCP surface adds full OAuth 2.0 with authorization code, client\n  credentials, and refresh/access-token flows, PKCE (S256), and dynamic client\n  registration (RFC 7591).\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer access token in the Authorization header for all product APIs.\n  applies_to: [scribe.kensho.com, extract.kensho.com,\
  \ nerd.kensho.com, kfinance.kensho.com]\n- name: PersonalToken\n  type: http\n  scheme: bearer\n  description: Development-time personal token issued from the Kensho services platform.\n  docs: https://docs.kensho.com/authentication/personal-token\n- name: KeyPair\n  type: http\n  scheme: bearer\n  description: >-\n    Production authentication using a client ID and private key pair that is\n    exchanged for a short-lived bearer access token.\n  docs: https://docs.kensho.com/authentication/keypair\n- name: OAuth2\n  type: oauth2\n  description: OAuth 2.0 for the LLM-ready API hosted MCP server.\n  issuer: https://kfinance.kensho.com/integrations\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://kfinance.kensho.com/integrations/authorize\n    tokenUrl: https://kfinance.kensho.com/integrations/token\n    registrationUrl: https://kfinance.kensho.com/integrations/register\n    pkce: S256\n  - flow: clientCredentials\n    tokenUrl: https://kfinance.kensho.com/integrations/token\n\
  \  - flow: refreshToken\n    tokenUrl: https://kfinance.kensho.com/integrations/token\n  token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\n  sources: [well-known/kensho-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kensho/refs/heads/main/authentication/kensho-authentication.yml
summary_line: http/oauth2 · 4 schemes
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Financial Data
- Speech to Text
- Transcription
- Document Extraction
- Named Entity Recognition
- Natural Language Processing
- LLM
- Model Context Protocol
- Retrieval
- S&P Global
---
