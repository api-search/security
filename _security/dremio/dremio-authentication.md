---
api_key_in:
- header
auth_types:
- http
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Dremio Authentication
name_suffix: Authentication
oauth_flows:
- tokenExchange
overview: Dremio secures its APIs with http, oauth2, and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the tokenExchange flow(s).
provider_name: Dremio
provider_slug: dremio
scheme_count: 4
schemes:
- description: Personal Access Token minted per user or service user; sent as a bearer token. The primary credential for scripts, the CLI, and the MCP server.
  format: Bearer <PAT>
  in: header
  name: PersonalAccessToken
  parameter: Authorization
  type: apiKey
- description: OAuth access token obtained by exchanging a PAT at login.dremio.cloud; Dremio recommends exchanging the PAT for an OAuth access token before production use.
  flow: tokenExchange
  name: OAuthAccessToken
  type: oauth2
- description: External JWT exchange lets an external IdP-issued token be exchanged for a Dremio token for federated / SSO connection types.
  name: ExternalJWT
  type: openIdConnect
- description: Console/web sign-in via SSO or username/password; third-party identity providers (Google, GitHub, IdP) are supported for account login.
  name: SSO
  type: sso
slug: dremio-authentication
source_filename: dremio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.dremio.com/dremio-cloud/security/authentication/\ndocs: https://docs.dremio.com/dremio-cloud/security/authentication/\nsummary:\n  types: [http, oauth2, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [tokenExchange]\n  transport: Authorization Bearer header on every REST request\nschemes:\n- name: PersonalAccessToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: \"Bearer <PAT>\"\n  description: >-\n    Personal Access Token minted per user or service user; sent as a bearer token.\n    The primary credential for scripts, the CLI, and the MCP server.\n- name: OAuthAccessToken\n  type: oauth2\n  flow: tokenExchange\n  description: >-\n    OAuth access token obtained by exchanging a PAT at login.dremio.cloud;\n    Dremio recommends exchanging the PAT for an OAuth access token before\n    production use.\n- name: ExternalJWT\n  type: openIdConnect\n  description: >-\n    External JWT exchange\
  \ lets an external IdP-issued token be exchanged for a\n    Dremio token for federated / SSO connection types.\n- name: SSO\n  type: sso\n  description: >-\n    Console/web sign-in via SSO or username/password; third-party identity\n    providers (Google, GitHub, IdP) are supported for account login.\nnotes:\n  - No OpenAPI is captured for this stub, so schemes are searched from the docs\n    auth page rather than derived from securitySchemes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dremio/refs/heads/main/authentication/dremio-authentication.yml
summary_line: http/oauth2/apiKey · 4 schemes
tags:
- Company
- Data Lakehouse
- Analytics
- SQL Query Engine
- Apache Iceberg
- Apache Arrow
- Data Catalog
- Semantic Layer
- AI Agents
- MCP
---
