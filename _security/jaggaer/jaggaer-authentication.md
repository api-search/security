---
api_key_in:
- header
api_specs:
- filename: jaggaer-async-api-openapi.yml
  format: yaml
  label: JAGGAER Async API
  slug: jaggaer-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-async-api-openapi.yml
- filename: jaggaer-attributes-api-openapi.yml
  format: yaml
  label: JAGGAER Attributes API
  slug: jaggaer-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-attributes-api-openapi.yml
- filename: jaggaer-awards-api-openapi.yml
  format: yaml
  label: JAGGAER Awards API
  slug: jaggaer-awards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-awards-api-openapi.yml
- filename: jaggaer-bids-api-openapi.yml
  format: yaml
  label: JAGGAER Bids API
  slug: jaggaer-bids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-bids-api-openapi.yml
- filename: jaggaer-contacts-api-openapi.yml
  format: yaml
  label: JAGGAER Contacts API
  slug: jaggaer-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-contacts-api-openapi.yml
- filename: jaggaer-customer-hosts-api-openapi.yml
  format: yaml
  label: JAGGAER Customer Hosts API
  slug: jaggaer-customer-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-customer-hosts-api-openapi.yml
- filename: jaggaer-events-api-openapi.yml
  format: yaml
  label: JAGGAER Events API
  slug: jaggaer-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-events-api-openapi.yml
- filename: jaggaer-items-api-openapi.yml
  format: yaml
  label: JAGGAER Items API
  slug: jaggaer-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-items-api-openapi.yml
- filename: jaggaer-jobs-api-openapi.yml
  format: yaml
  label: JAGGAER Jobs API
  slug: jaggaer-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-jobs-api-openapi.yml
- filename: jaggaer-locations-api-openapi.yml
  format: yaml
  label: JAGGAER Locations API
  slug: jaggaer-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-locations-api-openapi.yml
- filename: jaggaer-rates-api-openapi.yml
  format: yaml
  label: JAGGAER Rates API
  slug: jaggaer-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-rates-api-openapi.yml
- filename: jaggaer-scenarios-api-openapi.yml
  format: yaml
  label: JAGGAER Scenarios API
  slug: jaggaer-scenarios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-scenarios-api-openapi.yml
- filename: jaggaer-suppliers-api-openapi.yml
  format: yaml
  label: JAGGAER Suppliers API
  slug: jaggaer-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-suppliers-api-openapi.yml
- filename: jaggaer-templates-api-openapi.yml
  format: yaml
  label: JAGGAER Templates API
  slug: jaggaer-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-templates-api-openapi.yml
- filename: jaggaer-uploads-api-openapi.yml
  format: yaml
  label: JAGGAER Uploads API
  slug: jaggaer-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-uploads-api-openapi.yml
- filename: jaggaer-users-api-openapi.yml
  format: yaml
  label: JAGGAER Users API
  slug: jaggaer-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-users-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Jaggaer Authentication
name_suffix: Authentication
oauth_flows: []
overview: JAGGAER secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: JAGGAER
provider_slug: jaggaer
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 bearer token for authentication.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/jaggaer-aso-ches-openapi.yml
  - openapi/jaggaer-aso-ees-openapi.yml
  type: http
- description: API key passed as a request header.
  in: header
  name: apiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/jaggaer-aso-ches-openapi.yml
  - openapi/jaggaer-aso-ees-openapi.yml
  - openapi/jaggaer-aso-quay-openapi.yml
  type: apiKey
slug: jaggaer-authentication
source_filename: jaggaer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jaggaer-aso-ches-openapi.yml, openapi/jaggaer-aso-ees-openapi.yml, openapi/jaggaer-aso-quay-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token for authentication.\n  sources:\n  - openapi/jaggaer-aso-ches-openapi.yml\n  - openapi/jaggaer-aso-ees-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: API key passed as a request header.\n  sources:\n  - openapi/jaggaer-aso-ches-openapi.yml\n  - openapi/jaggaer-aso-ees-openapi.yml\n  - openapi/jaggaer-aso-quay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/authentication/jaggaer-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Procurement
- Sourcing
- Supplier Management
- Contracts
- Spend Analytics
- eProcurement
- Source-to-Pay
- Procure-to-Pay
---
