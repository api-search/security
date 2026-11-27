---
anonymous_access: false
api_key_in: []
api_specs:
- filename: honeylabs-net-bulk-api-openapi.yml
  format: yaml
  label: HoneyLabs Bulk API
  slug: honeylabs-net-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honeylabs-net/openapi/honeylabs-net-bulk-api-openapi.yml
- filename: honeylabs-net-lists-api-openapi.yml
  format: yaml
  label: HoneyLabs Lists API
  slug: honeylabs-net-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honeylabs-net/openapi/honeylabs-net-lists-api-openapi.yml
- filename: honeylabs-net-reports-api-openapi.yml
  format: yaml
  label: HoneyLabs Reports API
  slug: honeylabs-net-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honeylabs-net/openapi/honeylabs-net-reports-api-openapi.yml
- filename: honeylabs-net-service-api-openapi.yml
  format: yaml
  label: HoneyLabs Service API
  slug: honeylabs-net-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honeylabs-net/openapi/honeylabs-net-service-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: HoneyLabs Authentication
name_suffix: Authentication
oauth_flows: []
overview: HoneyLabs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HoneyLabs
provider_slug: honeylabs-net
scheme_count: 1
schemes:
- description: Free key from https://honeylabs.net/dashboard
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/honeylabs-net-openapi.json
  type: http
slug: honeylabs-net-authentication
source_filename: honeylabs-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/honeylabs-net-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Free key from https://honeylabs.net/dashboard\n  sources:\n  - openapi/honeylabs-net-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/honeylabs-net/authentication/honeylabs-net-authentication.yml
summary_line: http · 1 scheme
tags:
- Honeypot
- Threat Intelligence
- MCP
- Open Source
---
