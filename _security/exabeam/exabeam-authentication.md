---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Exabeam Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Exabeam secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Exabeam
provider_slug: exabeam
scheme_count: 1
schemes:
- description: Exabeam secures its REST APIs with OAuth2 bearer tokens. Developers generate an API Key and Secret in the console (Settings > API Keys); the Secret is shown in plaintext only once at creation. The key/secret pair is exchanged for a short-lived bearer access token at the regional token endpoint, which is then sent on API requests. The published RFC 8414 authorization-server metadata additionally advertises an authorization_code flow with PKCE (S256).
  flows:
  - flow: clientCredentials
    note: API key + secret exchanged for a bearer access token.
    tokenUrl: https://api.us-west.exabeam.cloud/oauth/token
  - authorizationUrl: https://api.us-west.exabeam.cloud/oauth/authorize
    flow: authorizationCode
    pkce: S256
    scopes:
      offline_access: Issue a refresh token for offline access
      openid: OpenID Connect authentication
      profile: Access to the authenticated principal's profile
    tokenUrl: https://api.us-west.exabeam.cloud/oauth/token
  name: OAuth2
  type: oauth2
slug: exabeam-authentication
source_filename: exabeam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.exabeam.com/exabeam/docs/api-keys\ndocs: https://developers.exabeam.com/exabeam/docs/api-keys\nwell_known: well-known/exabeam-oauth-authorization-server.json\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials, authorizationCode]\n  token_endpoint: https://api.us-west.exabeam.cloud/oauth/token\n  pkce: true\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    Exabeam secures its REST APIs with OAuth2 bearer tokens. Developers generate\n    an API Key and Secret in the console (Settings > API Keys); the Secret is\n    shown in plaintext only once at creation. The key/secret pair is exchanged\n    for a short-lived bearer access token at the regional token endpoint, which\n    is then sent on API requests. The published RFC 8414 authorization-server\n    metadata additionally advertises an authorization_code flow with PKCE (S256).\n  flows:\n  - flow: clientCredentials\n    tokenUrl:\
  \ https://api.us-west.exabeam.cloud/oauth/token\n    note: API key + secret exchanged for a bearer access token.\n  - flow: authorizationCode\n    authorizationUrl: https://api.us-west.exabeam.cloud/oauth/authorize\n    tokenUrl: https://api.us-west.exabeam.cloud/oauth/token\n    pkce: S256\n    scopes:\n      openid: OpenID Connect authentication\n      profile: Access to the authenticated principal's profile\n      offline_access: Issue a refresh token for offline access\nregional_endpoints:\n  token_endpoint_pattern: https://api.<region>.exabeam.cloud/oauth/token\n  regions: [us-west, us-east, eu, au, sg, jp, ca, ch]\nrate_limits:\n  authentication_api: 50 requests per 5 minutes per client source IP address\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exabeam/refs/heads/main/authentication/exabeam-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Cybersecurity
- Security
- SIEM
- UEBA
- Threat Detection
- Security Operations
- SOC
- Log Management
- Incident Response
---
