---
anonymous_access: false
api_key_in: []
api_specs:
- filename: frends-openapi-generated.yml
  format: yaml
  label: Frends API
  slug: frends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frends/refs/heads/main/openapi/_ae-authored/frends-openapi-generated.yml
auth_types: []
description: Authentication methods for Frends as documented.
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Frends Authentication
name_suffix: Authentication
oauth_flows: []
overview: Frends declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Frends
provider_slug: frends
scheme_count: 4
schemes:
- evidence: OAuth authentication for MCP Triggers is available from Frends 6.3.1 onwards.
  flows:
  - authorization_code
  how_to_obtain: Create an app registration in Microsoft Entra ID, add a Mobile and desktop applications platform, enable public client flows, and configure redirect URIs for clients. The flow uses authorization code with PKCE.
  name: Entra ID OAuth for MCP Triggers
  type: oauth2
- evidence: The easiest authentication method to use in Frends for APIs.
  how_to_obtain: Create an API key via Administration > API Keys in the Frends UI, then add it to an API Policy as an identity.
  name: API Key
  type: apiKey
- evidence: 'Basic Authentication method is based on a secret value in HTTP header. The header is in form Authorization: Basic "base64encode(username:password)"'
  header: Authorization
  how_to_obtain: Credentials are defined by the user (username and password) and encoded to Base64 for the Authorization header.
  location: header
  name: Basic Authentication
  type: http-basic
- evidence: How to use implicit OAuth 2.0 flow for your APIs in Frends.
  flows:
  - implicit
  how_to_obtain: Register an application in Microsoft Entra ID, configure a Web platform with a redirect URI ending in /api/auth/oauth2-redirect.html, and enable ID token issuance.
  name: Implicit OAuth flow for Frends APIs
  type: oauth2
slug: frends-authentication
source_filename: frends-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.frends.com/guides/ai-features/setting-up-entra-id-oauth-for-mcp-triggers.md
source_yaml: "generated: '2026-10-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.frends.com/guides/ai-features/setting-up-entra-id-oauth-for-mcp-triggers.md\nsources:\n- https://docs.frends.com/guides/ai-features/setting-up-entra-id-oauth-for-mcp-triggers.md\n- https://docs.frends.com/guides/api-management/how-to-create-and-use-api-keys-in-frends.md\n- https://docs.frends.com/guides/api-management/how-to-use-basic-authentication-for-apis-in-frends.md\n- https://docs.frends.com/guides/api-management/setting-up-implicit-oauth-flow-for-frends-apis.md\ndescription: Authentication methods for Frends as documented.\nschemes:\n- type: oauth2\n  name: Entra ID OAuth for MCP Triggers\n  evidence: OAuth authentication for MCP Triggers is available from Frends 6.3.1 onwards.\n  flows:\n  - authorization_code\n  how_to_obtain: Create an app registration in Microsoft Entra ID, add a Mobile and desktop applications platform, enable public client flows,\n    and\
  \ configure redirect URIs for clients. The flow uses authorization code with PKCE.\n- type: apiKey\n  name: API Key\n  evidence: The easiest authentication method to use in Frends for APIs.\n  how_to_obtain: Create an API key via Administration > API Keys in the Frends UI, then add it to an API Policy as an identity.\n- type: http-basic\n  name: Basic Authentication\n  evidence: 'Basic Authentication method is based on a secret value in HTTP header. The header is in form Authorization: Basic \"base64encode(username:password)\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Credentials are defined by the user (username and password) and encoded to Base64 for the Authorization header.\n- type: oauth2\n  name: Implicit OAuth flow for Frends APIs\n  evidence: How to use implicit OAuth 2.0 flow for your APIs in Frends.\n  flows:\n  - implicit\n  how_to_obtain: Register an application in Microsoft Entra ID, configure a Web platform with a redirect URI ending in /api/auth/oauth2-redirect.html,\n\
  \    and enable ID token issuance.\ndocs: https://docs.frends.com/guides/ai-features/setting-up-entra-id-oauth-for-mcp-triggers.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frends/refs/heads/main/authentication/frends-authentication.yml
summary_line: 4 schemes
tags:
- Integration
- iPaaS
- API Management
- Workflow Automation
- Enterprise Automation
- AI Orchestration
- Data Integration
- Hybrid Deployment - Integration - iPaaS
---
