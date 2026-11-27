---
anonymous_access: false
api_key_in: []
api_specs:
- filename: multi-upload-tool-com-accounts-api-openapi.yml
  format: yaml
  label: Multi Upload Tool Accounts API
  slug: multi-upload-tool-com-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multi-upload-tool-com/openapi/multi-upload-tool-com-accounts-api-openapi.yml
- filename: multi-upload-tool-com-ai-api-openapi.yml
  format: yaml
  label: Multi Upload Tool AI API
  slug: multi-upload-tool-com-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multi-upload-tool-com/openapi/multi-upload-tool-com-ai-api-openapi.yml
- filename: multi-upload-tool-com-analytics-api-openapi.yml
  format: yaml
  label: Multi Upload Tool Analytics API
  slug: multi-upload-tool-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multi-upload-tool-com/openapi/multi-upload-tool-com-analytics-api-openapi.yml
- filename: multi-upload-tool-com-domains-api-openapi.yml
  format: yaml
  label: Multi Upload Tool Domains API
  slug: multi-upload-tool-com-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multi-upload-tool-com/openapi/multi-upload-tool-com-domains-api-openapi.yml
- filename: multi-upload-tool-com-limits-api-openapi.yml
  format: yaml
  label: Multi Upload Tool Limits API
  slug: multi-upload-tool-com-limits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multi-upload-tool-com/openapi/multi-upload-tool-com-limits-api-openapi.yml
- filename: multi-upload-tool-com-pools-api-openapi.yml
  format: yaml
  label: Multi Upload Tool Pools API
  slug: multi-upload-tool-com-pools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multi-upload-tool-com/openapi/multi-upload-tool-com-pools-api-openapi.yml
- filename: multi-upload-tool-com-short-links-api-openapi.yml
  format: yaml
  label: Multi Upload Tool Short links API
  slug: multi-upload-tool-com-short-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multi-upload-tool-com/openapi/multi-upload-tool-com-short-links-api-openapi.yml
- filename: multi-upload-tool-com-teams-api-openapi.yml
  format: yaml
  label: Multi Upload Tool Teams API
  slug: multi-upload-tool-com-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multi-upload-tool-com/openapi/multi-upload-tool-com-teams-api-openapi.yml
- filename: multi-upload-tool-com-uploads-api-openapi.yml
  format: yaml
  label: Multi Upload Tool Uploads API
  slug: multi-upload-tool-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multi-upload-tool-com/openapi/multi-upload-tool-com-uploads-api-openapi.yml
- filename: multi-upload-tool-com-webhooks-api-openapi.yml
  format: yaml
  label: Multi Upload Tool Webhooks API
  slug: multi-upload-tool-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multi-upload-tool-com/openapi/multi-upload-tool-com-webhooks-api-openapi.yml
- filename: multi-upload-tool-com-white-label-api-openapi.yml
  format: yaml
  label: Multi Upload Tool White Label API
  slug: multi-upload-tool-com-white-label-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multi-upload-tool-com/openapi/multi-upload-tool-com-white-label-api-openapi.yml
auth_types: []
description: Authentication methods as published on the Multi Upload Tool documentation.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Multi Upload Tool Authentication
name_suffix: Authentication
oauth_flows: []
overview: Multi Upload Tool declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Multi Upload Tool
provider_slug: multi-upload-tool-com
scheme_count: 2
schemes:
- evidence: Sign in (OAuth) — Claude, ChatGPT and any spec‑compliant client
  header: Authorization
  how_to_obtain: The client discovers our authorization server, sends the user to a consent screen on Multi Upload Tool, and stores the returned token.
  location: header
  name: OAuth
  scopes:
  - mcp:read
  - mcp:write
  type: oauth2
- evidence: API keys on this endpoint are deprecated .
  header: x-api-key
  how_to_obtain: Generate a new API key in the dashboard under API Keys.
  location: header
  name: API Key
  type: apiKey
slug: multi-upload-tool-com-authentication
source_filename: multi-upload-tool-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.multi-upload-tool.com/mcp
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.multi-upload-tool.com/mcp\nsources:\n- https://docs.multi-upload-tool.com/mcp\n- https://docs.multi-upload-tool.com/get-started\ndescription: Authentication methods as published on the Multi Upload Tool documentation.\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Sign in (OAuth) — Claude, ChatGPT and any spec‑compliant client\n  location: header\n  header: Authorization\n  scopes:\n  - mcp:read\n  - mcp:write\n  how_to_obtain: The client discovers our authorization server, sends the user to a consent screen on Multi Upload Tool, and stores the returned\n    token.\n- type: apiKey\n  name: API Key\n  evidence: API keys on this endpoint are deprecated .\n  location: header\n  header: x-api-key\n  how_to_obtain: Generate a new API key in the dashboard under API Keys.\ndocs: https://docs.multi-upload-tool.com/mcp\n"
source_yaml_url: https://artifacts.apis.io/multi-upload-tool-com/authentication/multi-upload-tool-com-authentication.yml
summary_line: 2 schemes
tags:
- video publishing
- Social Media Scheduling
- Bulk Upload
- Analytics
---
