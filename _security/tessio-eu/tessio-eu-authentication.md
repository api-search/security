---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tessio-eu-age-verification-api-openapi.yml
  format: yaml
  label: tessio-eu Age Verification API
  slug: tessio-eu-age-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tessio-eu/openapi/tessio-eu-age-verification-api-openapi.yml
- filename: tessio-eu-stats-api-openapi.yml
  format: yaml
  label: tessio-eu Stats API
  slug: tessio-eu-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tessio-eu/openapi/tessio-eu-stats-api-openapi.yml
- filename: tessio-eu-webhooks-api-openapi.yml
  format: yaml
  label: tessio-eu Webhooks API
  slug: tessio-eu-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tessio-eu/openapi/tessio-eu-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Tessio Eu Authentication
name_suffix: Authentication
oauth_flows: []
overview: tessio-eu declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: tessio-eu
provider_slug: tessio-eu
scheme_count: 1
schemes:
- description: API key (tk_…) as Bearer token. Project key with scope 'full' accesses all routes; with 'stats:read' accesses only stats. Organisation key always 'stats:read'.
  scheme: bearer
  type: http
slug: tessio-eu-authentication
source_filename: tessio-eu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://tessio.eu/docs/api/\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"API key (tk_…) as Bearer token. Project key with scope 'full' accesses all routes; with 'stats:read' accesses only stats. Organisation key always 'stats:read'.\"\n"
source_yaml_url: https://artifacts.apis.io/tessio-eu/authentication/tessio-eu-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AgeVerification
- EU
- API
- Identity
---
