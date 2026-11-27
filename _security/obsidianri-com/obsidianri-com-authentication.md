---
anonymous_access: false
api_key_in: []
api_specs:
- filename: obsidianri-com-enforcement-api-openapi.yml
  format: yaml
  label: Obsidian Enforcement API
  slug: obsidianri-com-enforcement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obsidianri-com/openapi/obsidianri-com-enforcement-api-openapi.yml
- filename: obsidianri-com-health-api-openapi.yml
  format: yaml
  label: Obsidian Health API
  slug: obsidianri-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obsidianri-com/openapi/obsidianri-com-health-api-openapi.yml
- filename: obsidianri-com-monitoring-api-openapi.yml
  format: yaml
  label: Obsidian Monitoring API
  slug: obsidianri-com-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obsidianri-com/openapi/obsidianri-com-monitoring-api-openapi.yml
- filename: obsidianri-com-news-api-openapi.yml
  format: yaml
  label: Obsidian News API
  slug: obsidianri-com-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obsidianri-com/openapi/obsidianri-com-news-api-openapi.yml
- filename: obsidianri-com-reference-api-openapi.yml
  format: yaml
  label: Obsidian Reference API
  slug: obsidianri-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obsidianri-com/openapi/obsidianri-com-reference-api-openapi.yml
- filename: obsidianri-com-regulatory-api-openapi.yml
  format: yaml
  label: Obsidian Regulatory API
  slug: obsidianri-com-regulatory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obsidianri-com/openapi/obsidianri-com-regulatory-api-openapi.yml
- filename: obsidianri-com-standards-api-openapi.yml
  format: yaml
  label: Obsidian Standards API
  slug: obsidianri-com-standards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obsidianri-com/openapi/obsidianri-com-standards-api-openapi.yml
auth_types: []
description: Authentication schemes for Obsidian Enterprise API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Obsidian Authentication
name_suffix: Authentication
oauth_flows: []
overview: Obsidian declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Obsidian
provider_slug: obsidianri-com
scheme_count: 2
schemes:
- evidence: The enterprise API authenticates every request with an API key tied to your Obsidian account and plan.
  header: X-API-Key
  how_to_obtain: Create an API key from your Obsidian account under Account → API; the key is shown once at creation.
  location: header
  name: API Key
  type: apiKey
- evidence: 'Also supported: Authorization Bearer'
  header: Authorization
  how_to_obtain: Create an API key from your Obsidian account under Account → API; the key is shown once at creation.
  location: header
  name: Authorization Bearer
  type: apiKey
slug: obsidianri-com-authentication
source_filename: obsidianri-com-authentication.yml
source_heading: Authentication Profile
source_url: https://obsidianri.com/docs/api-authentication
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://obsidianri.com/docs/api-authentication\nsources:\n- https://obsidianri.com/docs/api-authentication\n- https://obsidianri.com/docs/quickstart\ndescription: Authentication schemes for Obsidian Enterprise API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: The enterprise API authenticates every request with an API key tied to your Obsidian account and plan.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create an API key from your Obsidian account under Account → API; the key is shown once at creation.\n- type: apiKey\n  name: Authorization Bearer\n  evidence: 'Also supported: Authorization Bearer'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key from your Obsidian account under Account → API; the key is shown once at creation.\nnote: No OAuth2, HTTP Basic, JWT, HMAC, MTLS, or other authentication schemes are documented.\n\
  docs: https://obsidianri.com/docs/api-authentication\n"
source_yaml_url: https://artifacts.apis.io/obsidianri-com/authentication/obsidianri-com-authentication.yml
summary_line: 2 schemes
tags:
- Regulatory
- Intelligence
- Compliance
- Monitoring
- Mapping
---
