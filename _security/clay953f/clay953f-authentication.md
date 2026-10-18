---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clay953f-credits-api-openapi.yml
  format: yaml
  label: Clay953f Credits API
  slug: clay953f-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clay953f/refs/heads/main/openapi/clay953f-credits-api-openapi.yml
- filename: clay953f-me-api-openapi.yml
  format: yaml
  label: Clay953f Me API
  slug: clay953f-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clay953f/refs/heads/main/openapi/clay953f-me-api-openapi.yml
- filename: clay953f-routines-api-openapi.yml
  format: yaml
  label: Clay953f Routines API
  slug: clay953f-routines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clay953f/refs/heads/main/openapi/clay953f-routines-api-openapi.yml
- filename: clay953f-search-api-openapi.yml
  format: yaml
  label: Clay953f Search API
  slug: clay953f-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clay953f/refs/heads/main/openapi/clay953f-search-api-openapi.yml
- filename: clay953f-tables-api-openapi.yml
  format: yaml
  label: Clay953f Tables API
  slug: clay953f-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clay953f/refs/heads/main/openapi/clay953f-tables-api-openapi.yml
- filename: clay953f-workflowsruns-api-openapi.yml
  format: yaml
  label: Clay953f Workflows Runs API
  slug: clay953f-workflowsruns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clay953f/refs/heads/main/openapi/clay953f-workflowsruns-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Clay953F Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clay953f declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Clay953f
provider_slug: clay953f
scheme_count: 1
schemes:
- evidence: Every request to the Clay Public API must include a Clay API key in the `clay-api-key` header.
  header: clay-api-key
  how_to_obtain: Create one under Settings → Account → API keys (beta) in the Clay UI.
  location: header
  name: Clay API Key
  type: apiKey
slug: clay953f-authentication
source_filename: clay953f-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.clay.com/public-api/authentication.md
source_yaml: "generated: '2026-10-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.clay.com/public-api/authentication.md\nsources:\n- https://developers.clay.com/public-api/authentication.md\n- https://university.clay.com/docs/http-api-with-jwt-authentication-integration-overview\n- https://university.clay.com/docs/guide-find-clay-api-key\n- https://university.clay.com/docs/oauth-optional-scopes\nschemes:\n- type: apiKey\n  name: Clay API Key\n  evidence: Every request to the Clay Public API must include a Clay API key in the `clay-api-key` header.\n  location: header\n  header: clay-api-key\n  how_to_obtain: Create one under Settings → Account → API keys (beta) in the Clay UI.\ndocs: https://developers.clay.com/public-api/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clay953f/refs/heads/main/authentication/clay953f-authentication.yml
summary_line: 1 scheme
tags:
- Data Marketplace
- CRM Enrichment
- AI Agents
---
