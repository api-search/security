---
api_key_in:
- header
auth_types:
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Impart Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Impart Security secures its APIs with http-bearer across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Impart Security
provider_slug: impart-security
scheme_count: 1
schemes:
- confirmed_scopes:
  - read:org_api_access_tokens
  description: Scoped API access token issued from the Impart console. Set as the IMPART_TOKEN environment variable (or a `token` argument) for the Terraform/Pulumi providers.
  issued_at: https://console.impartsecurity.net/ (Settings => Access Tokens)
  name: apiAccessToken
  scheme: bearer
  scope_model: 'Tokens are granted explicit scopes. read:org_api_access_tokens is required for the IaC providers to enumerate tokens; additional read:/write: scopes are granted per managed resource (specs, bindings, rules, lists, monitors, etc.).'
  type: http
slug: impart-security-authentication
source_filename: impart-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/impart-security/terraform-provider-impart (README + internal/apiclient), https://console.impartsecurity.net/\napi: Impart Security v0 REST API\nbase_url: https://api.impartsecurity.net/v0\nsummary:\n  types: [http-bearer]\n  api_key_in: [header]\n  model: >-\n    The Impart v0 REST API is authenticated with a scoped API access token\n    (\"IMPART_TOKEN\") issued from the Impart console under Settings => Access Tokens\n    => New API access token. Tokens are presented as a bearer credential and carry\n    read:/write: scopes granted per resource. The console web app itself is fronted\n    by an Auth0 OIDC tenant (auth.impartsecurity.net) for interactive human login.\nschemes:\n- name: apiAccessToken\n  type: http\n  scheme: bearer\n  description: >-\n    Scoped API access token issued from the Impart console. Set as the IMPART_TOKEN\n    environment variable (or a `token` argument) for the Terraform/Pulumi\
  \ providers.\n  issued_at: https://console.impartsecurity.net/ (Settings => Access Tokens)\n  scope_model: >-\n    Tokens are granted explicit scopes. read:org_api_access_tokens is required for\n    the IaC providers to enumerate tokens; additional read:/write: scopes are granted\n    per managed resource (specs, bindings, rules, lists, monitors, etc.).\n  confirmed_scopes:\n  - read:org_api_access_tokens\nconsole_identity:\n  provider: auth0\n  issuer: https://auth.impartsecurity.net/\n  authorization_endpoint: https://auth.impartsecurity.net/authorize\n  token_endpoint: https://auth.impartsecurity.net/oauth/token\n  grant_types: [authorization_code, client_credentials, refresh_token, urn:ietf:params:oauth:grant-type:token-exchange]\n  note: OIDC tenant for interactive console/docs login; distinct from the API access-token auth used by the REST API.\ndocs: https://docs.impartsecurity.net/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/impart-security/refs/heads/main/authentication/impart-security-authentication.yml
summary_line: http-bearer · 1 scheme
tags:
- Company
- Security
- API Security
- Runtime Protection
- WAF
- LLM Security
- AI Security
- MCP
- Agent Security
- Kong
- Governance
---
