---
api_key_in: []
api_specs:
- filename: shiftmove-custom-fields-api-openapi.yml
  format: yaml
  label: Shiftmove Custom fields API
  slug: shiftmove-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/openapi/shiftmove-custom-fields-api-openapi.yml
- filename: shiftmove-driver-assignments-api-openapi.yml
  format: yaml
  label: Shiftmove Driver assignments API
  slug: shiftmove-driver-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/openapi/shiftmove-driver-assignments-api-openapi.yml
- filename: shiftmove-drivers-api-openapi.yml
  format: yaml
  label: Shiftmove Drivers API
  slug: shiftmove-drivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/openapi/shiftmove-drivers-api-openapi.yml
- filename: shiftmove-invoices-api-openapi.yml
  format: yaml
  label: Shiftmove Invoices API
  slug: shiftmove-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/openapi/shiftmove-invoices-api-openapi.yml
- filename: shiftmove-organizations-api-openapi.yml
  format: yaml
  label: Shiftmove Organizations API
  slug: shiftmove-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/openapi/shiftmove-organizations-api-openapi.yml
- filename: shiftmove-vehicle-assignments-api-openapi.yml
  format: yaml
  label: Shiftmove Vehicle assignments API
  slug: shiftmove-vehicle-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/openapi/shiftmove-vehicle-assignments-api-openapi.yml
- filename: shiftmove-vehicle-financing-api-openapi.yml
  format: yaml
  label: Shiftmove Vehicle financing API
  slug: shiftmove-vehicle-financing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/openapi/shiftmove-vehicle-financing-api-openapi.yml
- filename: shiftmove-vehicle-license-plates-api-openapi.yml
  format: yaml
  label: Shiftmove Vehicle license plates API
  slug: shiftmove-vehicle-license-plates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/openapi/shiftmove-vehicle-license-plates-api-openapi.yml
- filename: shiftmove-vehicle-usages-api-openapi.yml
  format: yaml
  label: Shiftmove Vehicle usages API
  slug: shiftmove-vehicle-usages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/openapi/shiftmove-vehicle-usages-api-openapi.yml
- filename: shiftmove-vehicles-api-openapi.yml
  format: yaml
  label: Shiftmove Vehicles API
  slug: shiftmove-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/openapi/shiftmove-vehicles-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Shiftmove Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shiftmove secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shiftmove
provider_slug: shiftmove
scheme_count: 1
schemes:
- description: 'HTTP Basic authentication. Set `Authorization: Basic {base64(username:password)}` on every request. Documented in the Fleet-API "Access and usage / Authorization" section.'
  name: basicAuth
  scheme: basic
  sources:
  - docs
  type: http
slug: shiftmove-authentication
source_filename: shiftmove-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.avrios.com/\ndocs: https://developers.avrios.com/\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    The Avrios Fleet-API (the API surface of Shiftmove GmbH) uses HTTP Basic\n    authentication. A base64-encoded `username:password` credential pair must be\n    supplied on every request via the `Authorization: Basic {credentials}` header.\n    Credentials are issued by Avrios/Shiftmove per company account. The published\n    Swagger 2.0 document does not declare a `securityDefinitions` block, so this\n    profile is captured from the API documentation prose rather than derived from\n    the spec.\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic authentication. Set `Authorization: Basic {base64(username:password)}`\n      on every request. Documented in the Fleet-API \"Access and usage / Authorization\"\
  \n      section.\n    sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/authentication/shiftmove-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fleet Management
- Mobility
- Automotive
- Telematics
- Vehicles
- Fleet API
- SaaS
---
