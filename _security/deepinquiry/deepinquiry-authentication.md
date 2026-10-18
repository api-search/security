---
anonymous_access: false
api_key_in: []
api_specs:
- filename: deepinquiry-facts-api-openapi.yml
  format: yaml
  label: DeepInquiry Verified Facts API (Machine Accountability Corp) Facts API
  slug: deepinquiry-facts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepinquiry/refs/heads/main/openapi/deepinquiry-facts-api-openapi.yml
- filename: deepinquiry-search-api-openapi.yml
  format: yaml
  label: DeepInquiry Verified Facts API (Machine Accountability Corp) Search API
  slug: deepinquiry-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepinquiry/refs/heads/main/openapi/deepinquiry-search-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Deepinquiry Authentication
name_suffix: Authentication
oauth_flows: []
overview: DeepInquiry Verified Facts API (Machine Accountability Corp) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DeepInquiry Verified Facts API (Machine Accountability Corp)
provider_slug: deepinquiry
scheme_count: 1
schemes:
- evidence: 'Authentication: x-api-key: YOUR_API_KEY header.'
  header: x-api-key
  location: header
  name: x-api-key
  type: apiKey
slug: deepinquiry-authentication
source_filename: deepinquiry-authentication.yml
source_heading: Authentication Profile
source_url: https://www.deepinquiry.ai/docs
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.deepinquiry.ai/docs\nsources:\n- https://www.deepinquiry.ai/docs\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: 'Authentication: x-api-key: YOUR_API_KEY header.'\n  location: header\n  header: x-api-key\ndocs: https://www.deepinquiry.ai/docs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepinquiry/refs/heads/main/authentication/deepinquiry-authentication.yml
summary_line: 1 scheme
tags:
- Company
- API
- Facts
- Verification
- Data
---
