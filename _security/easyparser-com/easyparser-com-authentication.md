---
anonymous_access: false
api_key_in: []
api_specs:
- filename: easyparser-com-amazon-api-openapi.yml
  format: yaml
  label: easyparser-com Amazon API
  slug: easyparser-com-amazon-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easyparser-com/openapi/easyparser-com-amazon-api-openapi.yml
- filename: easyparser-com-bulk-api-openapi.yml
  format: yaml
  label: easyparser-com Bulk API
  slug: easyparser-com-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easyparser-com/openapi/easyparser-com-bulk-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Easyparser Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: easyparser-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: easyparser-com
provider_slug: easyparser-com
scheme_count: 2
schemes:
- description: Required by the documented realtime API. Inject secrets securely; do not expose request URLs in logs.
  in: query
  name: api_key
  type: apiKey
- description: Required by documented Bulk and Data Service endpoints.
  in: header
  name: api-key
  type: apiKey
slug: easyparser-com-authentication
source_filename: easyparser-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://easyparser.com/openapi.json\nschemes:\n  - type: apiKey\n    in: query\n    name: api_key\n    description: Required by the documented realtime API. Inject secrets securely; do not expose request URLs in logs.\n  - type: apiKey\n    in: header\n    name: api-key\n    description: Required by documented Bulk and Data Service endpoints.\n"
source_yaml_url: https://artifacts.apis.io/easyparser-com/authentication/easyparser-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- API
- Amazon
- Scraping
- Real-time
- Data-Extraction
---
