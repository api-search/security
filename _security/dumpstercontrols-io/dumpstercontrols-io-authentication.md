---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dumpstercontrols-io-customers-api-openapi.yml
  format: yaml
  label: Dumpster Controls Customers API
  slug: dumpstercontrols-io-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpstercontrols-io/openapi/dumpstercontrols-io-customers-api-openapi.yml
- filename: dumpstercontrols-io-estimates-api-openapi.yml
  format: yaml
  label: Dumpster Controls Estimates API
  slug: dumpstercontrols-io-estimates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpstercontrols-io/openapi/dumpstercontrols-io-estimates-api-openapi.yml
- filename: dumpstercontrols-io-junk-jobs-api-openapi.yml
  format: yaml
  label: Dumpster Controls Junk Jobs API
  slug: dumpstercontrols-io-junk-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpstercontrols-io/openapi/dumpstercontrols-io-junk-jobs-api-openapi.yml
- filename: dumpstercontrols-io-leads-api-openapi.yml
  format: yaml
  label: Dumpster Controls Leads API
  slug: dumpstercontrols-io-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpstercontrols-io/openapi/dumpstercontrols-io-leads-api-openapi.yml
- filename: dumpstercontrols-io-orders-api-openapi.yml
  format: yaml
  label: Dumpster Controls Orders API
  slug: dumpstercontrols-io-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpstercontrols-io/openapi/dumpstercontrols-io-orders-api-openapi.yml
- filename: dumpstercontrols-io-sizes-api-openapi.yml
  format: yaml
  label: Dumpster Controls Sizes API
  slug: dumpstercontrols-io-sizes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpstercontrols-io/openapi/dumpstercontrols-io-sizes-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Dumpster Controls Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dumpster Controls secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dumpster Controls
provider_slug: dumpstercontrols-io
scheme_count: 1
schemes:
- description: 'Send your API key as a Bearer token: Authorization: Bearer dc_live_... Keys are approved in Settings, API and must be kept secret (server-side only).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dumpstercontrols-io-openapi.json
  type: http
slug: dumpstercontrols-io-authentication
source_filename: dumpstercontrols-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/dumpstercontrols-io-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Send your API key as a Bearer token: Authorization: Bearer dc_live_... Keys\n    are approved in Settings, API and must be kept secret (server-side only).'\n  sources:\n  - openapi/dumpstercontrols-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/dumpstercontrols-io/authentication/dumpstercontrols-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Dumpster Controls
- Waste Management
- Software-as-a-Service
- Logistics
- FreeSoftware
---
