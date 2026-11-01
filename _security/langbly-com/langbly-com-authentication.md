---
anonymous_access: false
api_key_in: []
api_specs:
- filename: langbly-com-translation-api-openapi.yml
  format: yaml
  label: langbly-com Translation API
  slug: langbly-com-translation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/langbly-com/openapi/langbly-com-translation-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Langbly Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: langbly-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: langbly-com
provider_slug: langbly-com
scheme_count: 2
schemes:
- description: API key sent as X-API-Key header.
  in: header
  name: X-API-Key
  type: apiKey
- description: API key as query parameter (not recommended for production).
  in: query
  name: key
  type: apiKey
slug: langbly-com-authentication
source_filename: langbly-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://langbly.com/docs/authentication/\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: API key sent as X-API-Key header.\n  - type: apiKey\n    name: key\n    in: query\n    description: API key as query parameter (not recommended for production)."
source_yaml_url: https://artifacts.apis.io/langbly-com/authentication/langbly-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Translation
- API
- Localization
- SaaS
- Machine-Learning
---
