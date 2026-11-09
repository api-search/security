---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: daxoom-com-analytics-api-openapi.yml
  format: yaml
  label: Daxoom Analytics API
  slug: daxoom-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daxoom-com/openapi/daxoom-com-analytics-api-openapi.yml
- filename: daxoom-com-api-keys-api-openapi.yml
  format: yaml
  label: Daxoom API Keys API
  slug: daxoom-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daxoom-com/openapi/daxoom-com-api-keys-api-openapi.yml
- filename: daxoom-com-businesses-api-openapi.yml
  format: yaml
  label: Daxoom Businesses API
  slug: daxoom-com-businesses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daxoom-com/openapi/daxoom-com-businesses-api-openapi.yml
- filename: daxoom-com-categories-api-openapi.yml
  format: yaml
  label: Daxoom Categories API
  slug: daxoom-com-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daxoom-com/openapi/daxoom-com-categories-api-openapi.yml
- filename: daxoom-com-search-api-openapi.yml
  format: yaml
  label: Daxoom Search API
  slug: daxoom-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daxoom-com/openapi/daxoom-com-search-api-openapi.yml
- filename: daxoom-com-system-api-openapi.yml
  format: yaml
  label: Daxoom System API
  slug: daxoom-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daxoom-com/openapi/daxoom-com-system-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Daxoom Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Daxoom secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Daxoom
provider_slug: daxoom-com
scheme_count: 2
schemes:
- description: 'API key for the Public Query API. Get a free key at

    [app.daxoom.com/register](https://app.daxoom.com/register).

    Include in the `X-API-Key` header.'
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/daxoom-com-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: JWT access token obtained via login.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/daxoom-com-openapi.yml
  type: http
slug: daxoom-com-authentication
source_filename: daxoom-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/daxoom-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: |-\n    API key for the Public Query API. Get a free key at\n    [app.daxoom.com/register](https://app.daxoom.com/register).\n    Include in the `X-API-Key` header.\n  sources:\n  - openapi/daxoom-com-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT access token obtained via login.\n  sources:\n  - openapi/daxoom-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/daxoom-com/authentication/daxoom-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Local Business Data
- AI Agents
- Verified Profiles
- POS Integration
- Analytics
---
