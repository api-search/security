---
anonymous_access: false
api_key_in: []
api_specs:
- filename: leadmcp-ai-openapi-generated.yml
  format: yaml
  label: LeadMCP API
  slug: leadmcp-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadmcp-ai/openapi/_ae-authored/leadmcp-ai-openapi-generated.yml
auth_types: []
description: 'LeadMCP supports two authentication methods: an API key and OAuth 2.1.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: LeadMCP Authentication
name_suffix: Authentication
oauth_flows: []
overview: LeadMCP declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: LeadMCP
provider_slug: leadmcp-ai
scheme_count: 2
schemes:
- evidence: 'An API key on the Authorization header: Authorization: Bearer lm_live_... .'
  header: Authorization
  how_to_obtain: Create an API key via the Create an API key endpoint; the returned key is used as a Bearer token.
  location: header
  name: API Key
  type: apiKey
- evidence: Web connectors register dynamically and run the OAuth 2.1 authorization code flow with PKCE. Command line clients run the device authorization grant. Both send the resulting access token on the same Authorization header.
  flows:
  - authorization_code
  - device_authorization
  header: Authorization
  how_to_obtain: Obtain an access token via the OAuth 2.1 authorization code flow with PKCE (for web) or the device authorization grant (for CLI).
  location: header
  name: OAuth 2.1
  type: oauth2
slug: leadmcp-ai-authentication
source_filename: leadmcp-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.leadmcp.ai/authentication
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.leadmcp.ai/authentication\nsources:\n- https://docs.leadmcp.ai/authentication\n- https://docs.leadmcp.ai/keys/list-api-keys\n- https://docs.leadmcp.ai/keys/create-api-key\n- https://docs.leadmcp.ai/keys/revoke-api-key\ndescription: 'LeadMCP supports two authentication methods: an API key and OAuth 2.1.'\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'An API key on the Authorization header: Authorization: Bearer lm_live_... .'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key via the Create an API key endpoint; the returned key is used as a Bearer token.\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Web connectors register dynamically and run the OAuth 2.1 authorization code flow with PKCE. Command line clients run the device authorization\n    grant. Both send the resulting access token on the same Authorization header.\n  location:\
  \ header\n  header: Authorization\n  flows:\n  - authorization_code\n  - device_authorization\n  how_to_obtain: Obtain an access token via the OAuth 2.1 authorization code flow with PKCE (for web) or the device authorization grant (for CLI).\ndocs: https://docs.leadmcp.ai/authentication\n"
source_yaml_url: https://artifacts.apis.io/leadmcp-ai/authentication/leadmcp-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Sales
- Contacts
- B2B
- Lead Generation
---
