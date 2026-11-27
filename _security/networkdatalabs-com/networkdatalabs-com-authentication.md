---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: networkdatalabs-com-account-api-openapi.yml
  format: yaml
  label: Network Data Labs Account API
  slug: networkdatalabs-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/networkdatalabs-com/openapi/networkdatalabs-com-account-api-openapi.yml
- filename: networkdatalabs-com-asn-api-openapi.yml
  format: yaml
  label: Network Data Labs ASN API
  slug: networkdatalabs-com-asn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/networkdatalabs-com/openapi/networkdatalabs-com-asn-api-openapi.yml
- filename: networkdatalabs-com-bulk-api-openapi.yml
  format: yaml
  label: Network Data Labs Bulk API
  slug: networkdatalabs-com-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/networkdatalabs-com/openapi/networkdatalabs-com-bulk-api-openapi.yml
- filename: networkdatalabs-com-ip-lookup-api-openapi.yml
  format: yaml
  label: Network Data Labs IP Lookup API
  slug: networkdatalabs-com-ip-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/networkdatalabs-com/openapi/networkdatalabs-com-ip-lookup-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Network Data Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Network Data Labs secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Network Data Labs
provider_slug: networkdatalabs-com
scheme_count: 2
schemes:
- bearerFormat: API key
  description: 'API keys are issued by Network Data Labs. Prefer

    `Authorization: Bearer YOUR_API_KEY` (or `ndl_live_…` style keys).

    Unknown or missing keys return `401 UNAUTHORIZED`. Any non-empty

    string is **not** accepted.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/networkdatalabs-com-openapi.yml
  type: http
- description: Optional alternative to Bearer — useful for quick curl tests. Prefer header in production.
  in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/networkdatalabs-com-openapi.yml
  type: apiKey
slug: networkdatalabs-com-authentication
source_filename: networkdatalabs-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/networkdatalabs-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  description: |-\n    API keys are issued by Network Data Labs. Prefer\n    `Authorization: Bearer YOUR_API_KEY` (or `ndl_live_…` style keys).\n    Unknown or missing keys return `401 UNAUTHORIZED`. Any non-empty\n    string is **not** accepted.\n  sources:\n  - openapi/networkdatalabs-com-openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Optional alternative to Bearer — useful for quick curl tests. Prefer header in\n    production.\n  sources:\n  - openapi/networkdatalabs-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/networkdatalabs-com/authentication/networkdatalabs-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- IP Geolocation
- Network Intelligence
- Data
---
