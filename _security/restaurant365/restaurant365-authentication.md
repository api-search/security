---
api_key_in: []
api_specs:
- filename: restaurant365-r365-api-openapi.yml
  format: yaml
  label: R365 API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/openapi/restaurant365-r365-api-openapi.yml
- filename: restaurant365-odata-connector-openapi.yml
  format: yaml
  label: Restaurant365 OData Connector
  slug: odata-connector
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/openapi/restaurant365-odata-connector-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Restaurant365 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Restaurant365 secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Restaurant365
provider_slug: restaurant365
scheme_count: 2
schemes:
- description: Domain\Username with R365 password
  name: basicAuth
  scheme: basic
  sources:
  - openapi/restaurant365-odata-connector-openapi.yml
  type: http
- description: Bearer token returned by the Authenticate operation
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/restaurant365-r365-api-openapi.yml
  type: http
slug: restaurant365-authentication
source_filename: restaurant365-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/restaurant365-odata-connector-openapi.yml, openapi/restaurant365-r365-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Domain\\Username with R365 password\n  sources:\n  - openapi/restaurant365-odata-connector-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token returned by the Authenticate operation\n  sources:\n  - openapi/restaurant365-r365-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/authentication/restaurant365-authentication.yml
summary_line: http · 2 schemes
tags:
- Restaurant
- Accounting
- Inventory
- Operations
- Invoices
- Reporting
- OData
---
