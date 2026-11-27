---
anonymous_access: true
api_key_in: []
api_specs:
- filename: cukaimax-com-ask-api-openapi.yml
  format: yaml
  label: CukaiMax Ask API
  slug: cukaimax-com-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cukaimax-com/openapi/cukaimax-com-ask-api-openapi.yml
- filename: cukaimax-com-capabilities-api-openapi.yml
  format: yaml
  label: CukaiMax Capabilities API
  slug: cukaimax-com-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cukaimax-com/openapi/cukaimax-com-capabilities-api-openapi.yml
- filename: cukaimax-com-tax-reliefs-api-openapi.yml
  format: yaml
  label: CukaiMax Tax Reliefs API
  slug: cukaimax-com-tax-reliefs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cukaimax-com/openapi/cukaimax-com-tax-reliefs-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CukaiMax Authentication
name_suffix: Authentication
oauth_flows: []
overview: CukaiMax declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CukaiMax
provider_slug: cukaimax-com
scheme_count: 2
schemes:
- applies_to:
  - https://www.cukaimax.com/api/v1/*
  - https://www.cukaimax.com/.well-known/mcp
  - https://app.cukaimax.com/api/tax-authority/v1
  description: Public, anonymous, read-only. No API key is required.
  name: none
  type: none
- applies_to:
  - https://app.cukaimax.com/api/mcp
  consent_page: https://app.cukaimax.com/oauth/consent
  description: OAuth 2.1 through Supabase Auth, with dynamic client registration and PKCE. There is no API key.
  name: account-mcp-oauth
  protected_resource_metadata: https://app.cukaimax.com/.well-known/oauth-protected-resource/api/mcp
  standards:
  - RFC 9728
  type: oauth2
  unauthenticated_response: An unauthenticated request returns HTTP `401` with a `WWW-Authenticate` header pointing at the resource metadata.
slug: cukaimax-com-authentication
source_filename: cukaimax-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.cukaimax.com/mcp.md\ndocs: https://www.cukaimax.com/mcp.md#your-account-cukaimax-mcp\nnote: The OpenAPI (openapi.json) declares no securitySchemes; its three operations and the public Tax Authority MCP require no credentials (\"No API key is required\", https://www.cukaimax.com/developers.md). Only the account MCP is authenticated.\nschemes:\n- name: none\n  type: none\n  applies_to:\n  - https://www.cukaimax.com/api/v1/*\n  - https://www.cukaimax.com/.well-known/mcp\n  - https://app.cukaimax.com/api/tax-authority/v1\n  description: Public, anonymous, read-only. No API key is required.\n- name: account-mcp-oauth\n  type: oauth2\n  applies_to:\n  - https://app.cukaimax.com/api/mcp\n  description: OAuth 2.1 through Supabase Auth, with dynamic client registration and PKCE. There is no API key.\n  protected_resource_metadata: https://app.cukaimax.com/.well-known/oauth-protected-resource/api/mcp\n  consent_page: https://app.cukaimax.com/oauth/consent\n\
  \  unauthenticated_response: An unauthenticated request returns HTTP `401` with a `WWW-Authenticate` header pointing at the resource metadata.\n  standards:\n  - RFC 9728\n"
source_yaml_url: https://artifacts.apis.io/cukaimax-com/authentication/cukaimax-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Tax
- Personal Finance
- Malaysia
- Receipts
- Efiling
- MCP
- AI Agents
---
