---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: distribea-com-account-api-openapi.yml
  format: yaml
  label: Distribea Account API
  slug: distribea-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribea-com/openapi/distribea-com-account-api-openapi.yml
- filename: distribea-com-catalog-api-openapi.yml
  format: yaml
  label: Distribea Catalog API
  slug: distribea-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribea-com/openapi/distribea-com-catalog-api-openapi.yml
- filename: distribea-com-generation-api-openapi.yml
  format: yaml
  label: Distribea Generation API
  slug: distribea-com-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribea-com/openapi/distribea-com-generation-api-openapi.yml
- filename: distribea-com-models-api-openapi.yml
  format: yaml
  label: Distribea Models API
  slug: distribea-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribea-com/openapi/distribea-com-models-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Distribea Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Distribea secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Distribea
provider_slug: distribea-com
scheme_count: 2
schemes:
- description: Your Distribea key, from https://distribea.com/account/mcp.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/distribea-com-openapi.json
  type: http
- description: The same key, for clients that cannot set Authorization.
  in: header
  name: apiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/distribea-com-openapi.json
  type: apiKey
slug: distribea-com-authentication
source_filename: distribea-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/distribea-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Your Distribea key, from https://distribea.com/account/mcp.\n  sources:\n  - openapi/distribea-com-openapi.json\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: The same key, for clients that cannot set Authorization.\n  sources:\n  - openapi/distribea-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/distribea-com/authentication/distribea-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Artificial Intelligence
- Video
- Media
- Software-as-a-Service
- Platform
---
