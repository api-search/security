---
api_key_in:
- header
api_specs:
- filename: ryft-ingest-openapi.yml
  format: yaml
  label: Ryft Ingest API
  slug: ryft-ingest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryft/refs/heads/main/openapi/ryft-ingest-openapi.yml
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Ryft Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Ryft secures its APIs with apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Ryft
provider_slug: ryft
scheme_count: 3
schemes:
- description: Per-environment ingest token supplied by Ryft.
  in: header
  name: RyftIngestToken
  parameter: X-Ryft-Token
  sources:
  - openapi/ryft-ingest-openapi.yml
  type: apiKey
  used_by: Ryft Ingest API (ingest.ryft.io)
- authorization_endpoint: https://app.ryft.io/authorize
  code_challenge_methods:
  - S256
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  name: RyftMcpOAuth
  provider: Auth0
  registration_endpoint: https://app.ryft.io/register
  sources:
  - well-known/ryft-oauth-authorization-server.json
  token_endpoint: https://app.ryft.io/token
  type: oauth2
  used_by: Ryft MCP server (app.ryft.io/mcp) and the Ryft web app
- description: Organization single sign-on via Okta OIDC. Admins create an OIDC app, configure redirect URIs, and share credentials with Ryft.
  docs: https://docs.ryft.io/administration/okta-sso
  name: OktaSSO
  type: openIdConnect
  used_by: Ryft web app (organization login)
slug: ryft-authentication
source_filename: ryft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource:\n  - https://docs.ryft.io/integrations/custom-engine\n  - https://docs.ryft.io/integrations/ryft-mcp\n  - https://docs.ryft.io/administration/security-and-privacy\n  - https://docs.ryft.io/administration/okta-sso\ndocs: https://docs.ryft.io/administration/security-and-privacy\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  identity_provider: Auth0\n  sso: Okta OIDC (organization SSO)\nschemes:\n  - name: RyftIngestToken\n    type: apiKey\n    in: header\n    parameter: X-Ryft-Token\n    used_by: Ryft Ingest API (ingest.ryft.io)\n    description: Per-environment ingest token supplied by Ryft.\n    sources: [openapi/ryft-ingest-openapi.yml]\n  - name: RyftMcpOAuth\n    type: oauth2\n    flow: authorizationCode\n    authorization_endpoint: https://app.ryft.io/authorize\n    token_endpoint: https://app.ryft.io/token\n    registration_endpoint: https://app.ryft.io/register\n\
  \    code_challenge_methods: [S256]\n    grant_types: [authorization_code, refresh_token]\n    used_by: Ryft MCP server (app.ryft.io/mcp) and the Ryft web app\n    provider: Auth0\n    sources: [well-known/ryft-oauth-authorization-server.json]\n  - name: OktaSSO\n    type: openIdConnect\n    description: >-\n      Organization single sign-on via Okta OIDC. Admins create an OIDC app,\n      configure redirect URIs, and share credentials with Ryft.\n    used_by: Ryft web app (organization login)\n    docs: https://docs.ryft.io/administration/okta-sso\nnotes: >-\n  Cloud integrations (AWS/GCP/Azure/Snowflake/Databricks) use least-privilege,\n  read-only service accounts / IAM roles rather than end-user API auth.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ryft/refs/heads/main/authentication/ryft-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 3 schemes
tags:
- Company
- Data
- Data Lake
- Lakehouse
- Apache Iceberg
- Data Management
- Analytics
- Query Optimization
- AI
- MCP
---
