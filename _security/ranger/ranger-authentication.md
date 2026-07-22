---
api_key_in:
- environment
auth_types:
- oauth2
- openIdConnect
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Ranger Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- refreshToken
overview: Ranger secures its APIs with oauth2, openIdConnect, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, and refreshToken flow(s).
provider_name: Ranger
provider_slug: ranger
scheme_count: 3
schemes:
- description: Browser-based OAuth 2.0 / OIDC login is the default. The Ranger CLI opens a browser to authenticate and refreshes tokens automatically. Device-code and client-credentials grants support headless / CI use.
  name: oauth2-oidc
  sources:
  - https://login.ranger.net/.well-known/openid-configuration
  type: openIdConnect
- description: For CI / scripted / background-agent use, pass an API token (`ranger setup <token>`) or set the RANGER_CLI_TOKEN environment variable; the CLI reads it automatically.
  in: environment
  name: api-token
  parameter: RANGER_CLI_TOKEN
  sources:
  - https://docs.ranger.net/reference/cli-overview/
  type: apiKey
- description: The CLI can bootstrap auth via an MCP auth server (`ranger setup --mcp-bootstrap`, RANGER_MCP_AUTH_URL) so managed agent platforms and MCP-compatible tools can act on a real user's behalf without browser login.
  name: mcp-delegated
  sources:
  - https://docs.ranger.net/reference/cli-overview/
  type: oauth2
slug: ranger-authentication
source_filename: ranger-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://login.ranger.net/.well-known/openid-configuration\ndocs: https://docs.ranger.net/reference/cli-overview/\nsummary:\n  types: [oauth2, openIdConnect, apiKey]\n  oauth2_flows: [authorizationCode, clientCredentials, deviceCode, refreshToken]\n  api_key_in: [environment]\nissuer: https://login.ranger.net\noidc:\n  discovery: https://login.ranger.net/.well-known/openid-configuration\n  authorization_endpoint: https://login.ranger.net/oauth2/authorize\n  token_endpoint: https://login.ranger.net/oauth2/token\n  device_authorization_endpoint: https://login.ranger.net/oauth2/device_authorization\n  introspection_endpoint: https://login.ranger.net/oauth2/introspection\n  userinfo_endpoint: https://login.ranger.net/oauth2/userinfo\n  jwks_uri: https://login.ranger.net/oauth2/jwks\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  response_types_supported:\
  \ [code]\n  id_token_signing_alg_values_supported: [RS256]\n  token_endpoint_auth_methods_supported: [none, client_secret_basic, client_secret_post]\nschemes:\n- name: oauth2-oidc\n  type: openIdConnect\n  description: >-\n    Browser-based OAuth 2.0 / OIDC login is the default. The Ranger CLI opens a\n    browser to authenticate and refreshes tokens automatically. Device-code and\n    client-credentials grants support headless / CI use.\n  sources: [https://login.ranger.net/.well-known/openid-configuration]\n- name: api-token\n  type: apiKey\n  in: environment\n  parameter: RANGER_CLI_TOKEN\n  description: >-\n    For CI / scripted / background-agent use, pass an API token (`ranger setup\n    <token>`) or set the RANGER_CLI_TOKEN environment variable; the CLI reads it\n    automatically.\n  sources: [https://docs.ranger.net/reference/cli-overview/]\n- name: mcp-delegated\n  type: oauth2\n  description: >-\n    The CLI can bootstrap auth via an MCP auth server (`ranger setup\n    --mcp-bootstrap`,\
  \ RANGER_MCP_AUTH_URL) so managed agent platforms and\n    MCP-compatible tools can act on a real user's behalf without browser login.\n  sources: [https://docs.ranger.net/reference/cli-overview/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ranger/refs/heads/main/authentication/ranger-authentication.yml
summary_line: oauth2/openIdConnect/apiKey · 3 schemes
tags:
- Company
- Quality Assurance
- Testing
- Browser Automation
- Artificial Intelligence
- Agents
- Developer Tools
- DevOps
- CLI
---
