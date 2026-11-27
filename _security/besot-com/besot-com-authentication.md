---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: besot Authentication
name_suffix: Authentication
oauth_flows: []
overview: besot declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: besot
provider_slug: besot-com
scheme_count: 2
schemes:
- description: Your API key as a Bearer token. Get a free key at /developers.
  id: ApiKeyBearer
  scheme: bearer
  type: http
- description: Your API key (alternative to the Authorization header).
  id: ApiKeyHeader
  in: header
  name: x-api-key
  type: apiKey
slug: besot-com-authentication
source_filename: besot-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: https://besot.com/catalogue/openapi.json\nschemes:\n  - id: ApiKeyBearer\n    type: http\n    scheme: bearer\n    description: \"Your API key as a Bearer token. Get a free key at /developers.\"\n  - id: ApiKeyHeader\n    type: apiKey\n    in: header\n    name: x-api-key\n    description: \"Your API key (alternative to the Authorization header).\"\n"
source_yaml_url: https://artifacts.apis.io/besot-com/authentication/besot-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Fashion
- Resale
- Catalog
- Fandom
- Clothing
---
