---
anonymous_access: false
api_key_in: []
api_specs:
- filename: finology-tech-finology-publicapi-api-openapi.yml
  format: yaml
  label: finology-tech Finology.Public API
  slug: finology-tech-finology-publicapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finology-tech/openapi/finology-tech-finology-publicapi-api-openapi.yml
auth_types: []
description: Authentication methods for Finology Software API and MCP server
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Finology Tech Authentication
name_suffix: Authentication
oauth_flows: []
overview: finology-tech declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: finology-tech
provider_slug: finology-tech
scheme_count: 2
schemes:
- evidence: 'The REST API also accepts Authorization: Bearer <apiKey>.'
  header: Authorization
  how_to_obtain: Same as API Key – obtain apiKey via sandbox registration or production purchase.
  location: header
  name: Finology API Key Bearer
  type: http-bearer
- authorize_url: https://identity.finology.tech
  evidence: OAuth 2.1 authorization code with PKCE (S256). The authorization server is https://identity.finology.tech
  how_to_obtain: Sign in via the MCP server using the OAuth 2.1 authorization code flow with PKCE.
  name: Finology OAuth
  type: oauth2
slug: finology-tech-authentication
source_filename: finology-tech-authentication.yml
source_heading: Authentication Profile
source_url: https://finology.tech/auth.md
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://finology.tech/auth.md\nsources:\n- https://finology.tech/auth.md\ndescription: Authentication methods for Finology Software API and MCP server\nschemes:\n- type: http-bearer\n  name: Finology API Key Bearer\n  evidence: 'The REST API also accepts Authorization: Bearer <apiKey>.'\n  location: header\n  header: Authorization\n  how_to_obtain: Same as API Key – obtain apiKey via sandbox registration or production purchase.\n- type: oauth2\n  name: Finology OAuth\n  evidence: OAuth 2.1 authorization code with PKCE (S256). The authorization server is https://identity.finology.tech\n  authorize_url: https://identity.finology.tech\n  how_to_obtain: Sign in via the MCP server using the OAuth 2.1 authorization code flow with PKCE.\ndocs: https://finology.tech/auth.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/finology-tech/authentication/finology-tech-authentication.yml
summary_line: 2 schemes
tags:
- Company
- FinTech
- StudentLoans
- AIIntegration
- FinancialAdvisors
---
