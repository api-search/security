---
anonymous_access: false
api_key_in: []
api_specs:
- filename: prro-cloud-billing-api-openapi.yml
  format: yaml
  label: prro-cloud Billing API
  slug: prro-cloud-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prro-cloud/openapi/prro-cloud-billing-api-openapi.yml
- filename: prro-cloud-fiscal-api-openapi.yml
  format: yaml
  label: prro-cloud Fiscal API
  slug: prro-cloud-fiscal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prro-cloud/openapi/prro-cloud-fiscal-api-openapi.yml
- filename: prro-cloud-system-api-openapi.yml
  format: yaml
  label: prro-cloud System API
  slug: prro-cloud-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prro-cloud/openapi/prro-cloud-system-api-openapi.yml
- filename: prro-cloud-webhooks-api-openapi.yml
  format: yaml
  label: prro-cloud Webhooks API
  slug: prro-cloud-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prro-cloud/openapi/prro-cloud-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Prro Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: prro-cloud declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: prro-cloud
provider_slug: prro-cloud
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Machine-to-machine token issued in the PRRO.cloud cabinet, sent in Authorization header.
  scheme: bearer
  type: http
slug: prro-cloud-authentication
source_filename: prro-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://prro.cloud/docs/api/\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Machine-to-machine token issued in the PRRO.cloud cabinet, sent in Authorization header.\n"
source_yaml_url: https://artifacts.apis.io/prro-cloud/authentication/prro-cloud-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Payments
- Fiscal
- API
- Ukraine
---
