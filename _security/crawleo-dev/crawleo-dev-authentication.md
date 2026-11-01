---
anonymous_access: false
api_key_in: []
api_specs:
- filename: crawleo-dev-crawl-api-openapi.yml
  format: yaml
  label: crawleo-dev Crawl API
  slug: crawleo-dev-crawl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawleo-dev/openapi/crawleo-dev-crawl-api-openapi.yml
- filename: crawleo-dev-google-maps-api-openapi.yml
  format: yaml
  label: crawleo-dev Google Maps API
  slug: crawleo-dev-google-maps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawleo-dev/openapi/crawleo-dev-google-maps-api-openapi.yml
- filename: crawleo-dev-search-api-openapi.yml
  format: yaml
  label: crawleo-dev Search API
  slug: crawleo-dev-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawleo-dev/openapi/crawleo-dev-search-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Crawleo Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: crawleo-dev declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: crawleo-dev
provider_slug: crawleo-dev
scheme_count: 2
schemes:
- description: 'Bearer token format: Authorization: Bearer YOUR_API_KEY'
  in: header
  name: Authorization
  type: apiKey
- description: Header x-api-key with your API key
  in: header
  name: x-api-key
  type: apiKey
slug: crawleo-dev-authentication
source_filename: crawleo-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://docs.crawleo.dev/authentication.md\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Bearer token format: Authorization: Bearer YOUR_API_KEY\"\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: \"Header x-api-key with your API key\"\n"
source_yaml_url: https://artifacts.apis.io/crawleo-dev/authentication/crawleo-dev-authentication.yml
summary_line: 2 schemes
tags:
- AI
- Search
- Crawling
- API
- MCP
---
