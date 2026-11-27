---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: gajo-io-a-b-templates-api-openapi.yml
  format: yaml
  label: Gajo A/B Templates API
  slug: gajo-io-a-b-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gajo-io/openapi/gajo-io-a-b-templates-api-openapi.yml
- filename: gajo-io-account-api-openapi.yml
  format: yaml
  label: Gajo Account API
  slug: gajo-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gajo-io/openapi/gajo-io-account-api-openapi.yml
- filename: gajo-io-analytics-api-openapi.yml
  format: yaml
  label: Gajo Analytics API
  slug: gajo-io-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gajo-io/openapi/gajo-io-analytics-api-openapi.yml
- filename: gajo-io-app-links-api-openapi.yml
  format: yaml
  label: Gajo App Links API
  slug: gajo-io-app-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gajo-io/openapi/gajo-io-app-links-api-openapi.yml
- filename: gajo-io-bindings-api-openapi.yml
  format: yaml
  label: Gajo Bindings API
  slug: gajo-io-bindings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gajo-io/openapi/gajo-io-bindings-api-openapi.yml
- filename: gajo-io-route-templates-api-openapi.yml
  format: yaml
  label: Gajo Route Templates API
  slug: gajo-io-route-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gajo-io/openapi/gajo-io-route-templates-api-openapi.yml
- filename: gajo-io-routing-rules-api-openapi.yml
  format: yaml
  label: Gajo Routing Rules API
  slug: gajo-io-routing-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gajo-io/openapi/gajo-io-routing-rules-api-openapi.yml
- filename: gajo-io-urls-api-openapi.yml
  format: yaml
  label: Gajo URLs API
  slug: gajo-io-urls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gajo-io/openapi/gajo-io-urls-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Gajo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gajo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gajo
provider_slug: gajo-io
scheme_count: 1
schemes:
- description: Your Gajo API key. Generate one on the API Keys page of your account (https://gajo.io/account/keys).
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/gajo-io-openapi.json
  type: apiKey
slug: gajo-io-authentication
source_filename: gajo-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/gajo-io-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Your Gajo API key. Generate one on the API Keys page of your account (https://gajo.io/account/keys).\n  sources:\n  - openapi/gajo-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/gajo-io/authentication/gajo-io-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- URL Shorteners
- Analytics
- Developer Tool
---
