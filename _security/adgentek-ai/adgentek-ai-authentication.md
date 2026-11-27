---
anonymous_access: false
api_key_in: []
api_specs:
- filename: adgentek-ai-advertiser-api-openapi.yml
  format: yaml
  label: Adgentek Advertiser API
  slug: adgentek-ai-advertiser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adgentek-ai/openapi/adgentek-ai-advertiser-api-openapi.yml
- filename: adgentek-ai-meta-api-openapi.yml
  format: yaml
  label: Adgentek Meta API
  slug: adgentek-ai-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adgentek-ai/openapi/adgentek-ai-meta-api-openapi.yml
- filename: adgentek-ai-publisher-api-openapi.yml
  format: yaml
  label: Adgentek Publisher API
  slug: adgentek-ai-publisher-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adgentek-ai/openapi/adgentek-ai-publisher-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Adgentek Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adgentek declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Adgentek
provider_slug: adgentek-ai
scheme_count: 3
schemes:
- audience: advertiser
  description: Advertiser API key (advertiser_api_keys)
  in: header
  name: x-api-key
  type: apiKey
- audience: publisher
  description: Publisher API key (publisher_api_keys)
  in: header
  name: x-api-key
  type: apiKey
- audience: admin
  description: Super-admin service token (admin_service_tokens)
  in: header
  name: x-admin-token
  type: apiKey
slug: adgentek-ai-authentication
source_filename: adgentek-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://api.adgentek.ai/webapi/openapi.yaml\nschemes:\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: Advertiser API key (advertiser_api_keys)\n    audience: advertiser\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: Publisher API key (publisher_api_keys)\n    audience: publisher\n  - type: apiKey\n    name: x-admin-token\n    in: header\n    description: Super-admin service token (admin_service_tokens)\n    audience: admin\n"
source_yaml_url: https://artifacts.apis.io/adgentek-ai/authentication/adgentek-ai-authentication.yml
summary_line: 3 schemes
tags:
- Advertising
- Artificial Intelligence
- AdTech
- AI Agents
- Monetization
- Servers
---
