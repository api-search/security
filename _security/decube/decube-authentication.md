---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Decube Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Decube secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Decube
provider_slug: decube
scheme_count: 3
schemes:
- applies_to:
  - Data API
  - Control API
  in: header
  name: X-Decube-Api-Key
  parameter_name: X-Decube-Api-Key
  source: https://docs.decube.io/public-api/api-keys
  type: apiKey
- applies_to:
  - MCP Server
  flow: authorizationCode
  name: OAuth2
  source: https://docs.decube.io/mcp/quick-start
  type: oauth2
- applies_to:
  - Web application sign-in
  name: SSO / MFA
  source: https://docs.decube.io/org-settings/multi-factor-authentication
  type: platform
slug: decube-authentication
source_filename: decube-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.decube.io/public-api/overview\ndocs: https://docs.decube.io/public-api/api-keys\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nnotes: >-\n  The Decube Public REST API (Data API + Control API) authenticates with a static API key sent in the\n  X-Decube-Api-Key request header. API access is opt-in per organization (enabled by Sales / Account\n  Manager) and limited to Owner-level users; each user may hold up to 5 active API keys, generated from\n  My Account -> Update Profile -> Generate New API Key. The hosted MCP server uses OAuth 2.0 instead of\n  the API key. Platform (UI) sign-in supports SSO and multi-factor authentication.\nschemes:\n- name: X-Decube-Api-Key\n  type: apiKey\n  in: header\n  parameter_name: X-Decube-Api-Key\n  applies_to: [Data API, Control API]\n  source: https://docs.decube.io/public-api/api-keys\n- name: OAuth2\n  type: oauth2\n  flow:\
  \ authorizationCode\n  applies_to: [MCP Server]\n  source: https://docs.decube.io/mcp/quick-start\n- name: SSO / MFA\n  type: platform\n  applies_to: [Web application sign-in]\n  source: https://docs.decube.io/org-settings/multi-factor-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/decube/refs/heads/main/authentication/decube-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Data Observability
- Data Governance
- Data Catalog
- Data Quality
- Data Lineage
- Metadata Management
- Data Trust
- Data Products
- Model Context Protocol
---
