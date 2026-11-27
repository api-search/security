---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hostilo-app-files-api-openapi.yml
  format: yaml
  label: Hostilo Files API
  slug: hostilo-app-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hostilo-app/openapi/hostilo-app-files-api-openapi.yml
- filename: hostilo-app-sites-api-openapi.yml
  format: yaml
  label: Hostilo Sites API
  slug: hostilo-app-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hostilo-app/openapi/hostilo-app-sites-api-openapi.yml
- filename: hostilo-app-statistics-api-openapi.yml
  format: yaml
  label: Hostilo Statistics API
  slug: hostilo-app-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hostilo-app/openapi/hostilo-app-statistics-api-openapi.yml
- filename: hostilo-app-templates-api-openapi.yml
  format: yaml
  label: Hostilo Templates API
  slug: hostilo-app-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hostilo-app/openapi/hostilo-app-templates-api-openapi.yml
- filename: hostilo-app-versions-api-openapi.yml
  format: yaml
  label: Hostilo Versions API
  slug: hostilo-app-versions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hostilo-app/openapi/hostilo-app-versions-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hostilo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hostilo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Hostilo
provider_slug: hostilo-app
scheme_count: 1
schemes:
- description: Bearer token generated in Dashboard > API & tools. Starts with hk_...
  in: header
  name: Authorization
  type: apiKey
slug: hostilo-app-authentication
source_filename: hostilo-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: searched\nsource: https://hostilo.app/docs#agents_content\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: Bearer token generated in Dashboard > API & tools. Starts with hk_...\n"
source_yaml_url: https://artifacts.apis.io/hostilo-app/authentication/hostilo-app-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Hosting
- Artificial Intelligence
- Free
- Static
---
