---
api_key_in:
- header
api_specs:
- filename: tabs-external-api-openapi.yml
  format: yaml
  label: Tabs External API
  slug: tabs-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabs/refs/heads/main/openapi/tabs-external-api-openapi.yml
- filename: tabs-usage-api-beta-openapi.yml
  format: yaml
  label: Tabs Usage API (Beta)
  slug: tabs-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabs/refs/heads/main/openapi/tabs-usage-api-beta-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Tabs Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
overview: Tabs secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and deviceCode flow(s).
provider_name: Tabs
provider_slug: tabs
scheme_count: 2
schemes:
- format: 'Authorization: <API_KEY> (Usage API docs also show ''Authorization: Bearer <your-key>'')'
  in: header
  issuance: Admins generate API keys in the Developers section of the Tabs app side navigation; non-admins must request one from their Tabs administrator. Keys identify the merchant and the scopes they may access; revocation takes effect after eviction from an hourly cache. Self-service key rotation is on the roadmap per the docs.
  name: custom-header
  parameter: Authorization
  sources:
  - openapi/tabs-external-api-openapi.yml
  - openapi/tabs-usage-api-beta-openapi.yml
  type: apiKey
- description: OAuth 2.0 (WorkOS-backed) protects the Tabs MCP server at https://integrators.prod.api.tabsplatform.com/mcp — not the REST API, which is API-key only. Standard discovery via RFC 8414 + RFC 9728 metadata; PKCE S256; dynamic client registration; automatic merchant scoping.
  flows:
  - authorizationUrl: https://login.tabs.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.tabs.com/oauth2/token
  - authorizationUrl: https://login.tabs.com/oauth2/device_authorization
    flow: deviceCode
    tokenUrl: https://login.tabs.com/oauth2/token
  name: mcp-oauth
  scopes_supported:
  - openid
  - profile
  - email
  - offline_access
  sources:
  - well-known/tabs-oauth-authorization-server.json
  - well-known/tabs-mcp-oauth-protected-resource.json
  - well-known/tabs-openid-configuration.json
  type: oauth2
slug: tabs-authentication
source_filename: tabs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/tabs-external-api-openapi.yml, openapi/tabs-usage-api-beta-openapi.yml\ndocs: https://docs.tabsplatform.com/docs/authentication\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - deviceCode\nschemes:\n- name: custom-header\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: \"Authorization: <API_KEY> (Usage API docs also show 'Authorization: Bearer <your-key>')\"\n  issuance: >-\n    Admins generate API keys in the Developers section of the Tabs app side\n    navigation; non-admins must request one from their Tabs administrator.\n    Keys identify the merchant and the scopes they may access; revocation\n    takes effect after eviction from an hourly cache. Self-service key\n    rotation is on the roadmap per the docs.\n  sources:\n  - openapi/tabs-external-api-openapi.yml\n  - openapi/tabs-usage-api-beta-openapi.yml\n- name: mcp-oauth\n\
  \  type: oauth2\n  description: >-\n    OAuth 2.0 (WorkOS-backed) protects the Tabs MCP server at\n    https://integrators.prod.api.tabsplatform.com/mcp — not the REST API,\n    which is API-key only. Standard discovery via RFC 8414 + RFC 9728\n    metadata; PKCE S256; dynamic client registration; automatic merchant\n    scoping.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.tabs.com/oauth2/authorize\n    tokenUrl: https://login.tabs.com/oauth2/token\n  - flow: deviceCode\n    authorizationUrl: https://login.tabs.com/oauth2/device_authorization\n    tokenUrl: https://login.tabs.com/oauth2/token\n  scopes_supported: [openid, profile, email, offline_access]\n  sources:\n  - well-known/tabs-oauth-authorization-server.json\n  - well-known/tabs-mcp-oauth-protected-resource.json\n  - well-known/tabs-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabs/refs/heads/main/authentication/tabs-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Billing
- Revenue Automation
- Accounts Receivable
- Revenue Recognition
- Usage-Based Billing
- Invoicing
- Collections
- Fintech
- SaaS
---
