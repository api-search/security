---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hyperaware-live-trends-api-openapi.yml
  format: yaml
  label: Hyperaware Trends API
  slug: hyperaware-live-trends-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperaware-live/openapi/hyperaware-live-trends-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hyperaware Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hyperaware declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Hyperaware
provider_slug: hyperaware-live
scheme_count: 1
schemes:
- evidence: 'Send your key in the Authorization header: Bearer YOUR_API_KEY (the bare key works too).'
  header: Authorization
  location: header
  name: API key
  type: apiKey
slug: hyperaware-live-authentication
source_filename: hyperaware-live-authentication.yml
source_heading: Authentication Profile
source_url: https://hyperaware.live/docs/mcp
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://hyperaware.live/docs/mcp\nsources:\n- https://hyperaware.live/docs/mcp\ndescription: Authentication\nschemes:\n- type: apiKey\n  name: API key\n  evidence: 'Send your key in the Authorization header: Bearer YOUR_API_KEY (the bare key works too).'\n  location: header\n  header: Authorization\nnote: OAuth authentication is mentioned for Claude, ChatGPT, and other connectors, but no token or authorize URLs, flows, or scopes are provided\n  on the page.\ndocs: https://hyperaware.live/docs/mcp\n"
source_yaml_url: https://artifacts.apis.io/hyperaware-live/authentication/hyperaware-live-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Trending
- Aggregator
- Data
---
