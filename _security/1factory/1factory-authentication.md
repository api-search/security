---
api_key_in:
- header
api_specs:
- filename: 1factory-customers-api-openapi.yml
  format: yaml
  label: 1Factory Customers API
  slug: 1factory-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/openapi/1factory-customers-api-openapi.yml
- filename: 1factory-manufacturing-api-openapi.yml
  format: yaml
  label: 1Factory Manufacturing API
  slug: 1factory-manufacturing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/openapi/1factory-manufacturing-api-openapi.yml
- filename: 1factory-part-master-api-openapi.yml
  format: yaml
  label: 1Factory Part Master API
  slug: 1factory-part-master-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/openapi/1factory-part-master-api-openapi.yml
- filename: 1factory-qms-api-openapi.yml
  format: yaml
  label: 1Factory QMS API
  slug: 1factory-qms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/openapi/1factory-qms-api-openapi.yml
- filename: 1factory-receiving-api-openapi.yml
  format: yaml
  label: 1Factory Receiving API
  slug: 1factory-receiving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/openapi/1factory-receiving-api-openapi.yml
- filename: 1factory-suppliers-api-openapi.yml
  format: yaml
  label: 1Factory Suppliers API
  slug: 1factory-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/openapi/1factory-suppliers-api-openapi.yml
- filename: 1factory-work-orders-api-openapi.yml
  format: yaml
  label: 1Factory Work Orders API
  slug: 1factory-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/openapi/1factory-work-orders-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: 1Factory Authentication
name_suffix: Authentication
oauth_flows: []
overview: 1Factory secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: 1Factory
provider_slug: 1factory
scheme_count: 2
schemes:
- description: ID of your organization in 1Factory. Available in the Settings page of the 1Factory application.
  in: header
  name: OrgId
  parameter: x-1factory-org
  sources:
  - openapi/1factory-openapi.json
  type: apiKey
- description: API key for your organization. Generated in the Settings page of the 1Factory application.
  in: header
  name: ApiKey
  parameter: x-1factory-key
  sources:
  - openapi/1factory-openapi.json
  type: apiKey
slug: 1factory-authentication
source_filename: 1factory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/1factory-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: OrgId\n  type: apiKey\n  in: header\n  parameter: x-1factory-org\n  description: ID of your organization in 1Factory. Available in the Settings page of the 1Factory\n    application.\n  sources:\n  - openapi/1factory-openapi.json\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: x-1factory-key\n  description: API key for your organization. Generated in the Settings page of the 1Factory\n    application.\n  sources:\n  - openapi/1factory-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/authentication/1factory-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
---
