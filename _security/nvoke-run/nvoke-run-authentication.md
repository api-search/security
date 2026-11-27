---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nvoke-run-account-api-openapi.yml
  format: yaml
  label: nvoke Account API
  slug: nvoke-run-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nvoke-run/openapi/nvoke-run-account-api-openapi.yml
- filename: nvoke-run-agents-api-openapi.yml
  format: yaml
  label: nvoke Agents API
  slug: nvoke-run-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nvoke-run/openapi/nvoke-run-agents-api-openapi.yml
- filename: nvoke-run-api-keys-api-openapi.yml
  format: yaml
  label: nvoke API keys API
  slug: nvoke-run-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nvoke-run/openapi/nvoke-run-api-keys-api-openapi.yml
- filename: nvoke-run-drops-api-openapi.yml
  format: yaml
  label: nvoke Drops API
  slug: nvoke-run-drops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nvoke-run/openapi/nvoke-run-drops-api-openapi.yml
- filename: nvoke-run-leads-api-openapi.yml
  format: yaml
  label: nvoke Leads API
  slug: nvoke-run-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nvoke-run/openapi/nvoke-run-leads-api-openapi.yml
- filename: nvoke-run-meta-api-openapi.yml
  format: yaml
  label: nvoke Meta API
  slug: nvoke-run-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nvoke-run/openapi/nvoke-run-meta-api-openapi.yml
- filename: nvoke-run-privacy-api-openapi.yml
  format: yaml
  label: nvoke Privacy API
  slug: nvoke-run-privacy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nvoke-run/openapi/nvoke-run-privacy-api-openapi.yml
- filename: nvoke-run-searches-api-openapi.yml
  format: yaml
  label: nvoke Searches API
  slug: nvoke-run-searches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nvoke-run/openapi/nvoke-run-searches-api-openapi.yml
- filename: nvoke-run-tools-api-openapi.yml
  format: yaml
  label: nvoke Tools API
  slug: nvoke-run-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nvoke-run/openapi/nvoke-run-tools-api-openapi.yml
- filename: nvoke-run-webhooks-api-openapi.yml
  format: yaml
  label: nvoke Webhooks API
  slug: nvoke-run-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nvoke-run/openapi/nvoke-run-webhooks-api-openapi.yml
auth_types: []
description: Authentication methods for nvoke API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: nvoke Authentication
name_suffix: Authentication
oauth_flows: []
overview: nvoke declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: nvoke
provider_slug: nvoke-run
scheme_count: 2
schemes:
- evidence: 'Send Authorization: Bearer nvk_sk_... as a header.'
  header: Authorization
  location: header
  name: API Key
  type: apiKey
- evidence: OAuth. Clients that speak MCP OAuth need only the URL. The first call answers 401 and points the client at nvoke’s sign-in.
  name: OAuth
  type: oauth2
slug: nvoke-run-authentication
source_filename: nvoke-run-authentication.yml
source_heading: Authentication Profile
source_url: https://nvoke.run/docs
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://nvoke.run/docs\nsources:\n- https://nvoke.run/docs\n- https://nvoke.run/docs/mcp\ndescription: Authentication methods for nvoke API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Send Authorization: Bearer nvk_sk_... as a header.'\n  location: header\n  header: Authorization\n- type: oauth2\n  name: OAuth\n  evidence: OAuth. Clients that speak MCP OAuth need only the URL. The first call answers 401 and points the client at nvoke’s sign-in.\ndocs: https://nvoke.run/docs\n"
source_yaml_url: https://artifacts.apis.io/nvoke-run/authentication/nvoke-run-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Email Verification
- Data Enrichment
- Software-as-a-Service
- Privacy
---
