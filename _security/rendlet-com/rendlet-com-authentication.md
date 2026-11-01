---
anonymous_access: false
api_key_in: []
api_specs:
- filename: rendlet-com-checkout-api-openapi.yml
  format: yaml
  label: rendlet-com Checkout API
  slug: rendlet-com-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendlet-com/openapi/rendlet-com-checkout-api-openapi.yml
- filename: rendlet-com-pdf-api-openapi.yml
  format: yaml
  label: rendlet-com PDF API
  slug: rendlet-com-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendlet-com/openapi/rendlet-com-pdf-api-openapi.yml
- filename: rendlet-com-signup-api-openapi.yml
  format: yaml
  label: rendlet-com Signup API
  slug: rendlet-com-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendlet-com/openapi/rendlet-com-signup-api-openapi.yml
- filename: rendlet-com-templates-api-openapi.yml
  format: yaml
  label: rendlet-com Templates API
  slug: rendlet-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendlet-com/openapi/rendlet-com-templates-api-openapi.yml
- filename: rendlet-com-usage-api-openapi.yml
  format: yaml
  label: rendlet-com Usage API
  slug: rendlet-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendlet-com/openapi/rendlet-com-usage-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Rendlet Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: rendlet-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: rendlet-com
provider_slug: rendlet-com
scheme_count: 2
schemes:
- description: Bearer token in Authorization header.
  scheme: bearer
  type: http
- description: API key passed in X-API-Key header.
  in: header
  name: X-API-Key
  type: apiKey
slug: rendlet-com-authentication
source_filename: rendlet-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://rendlet.com/guides/html-to-pdf-node\nschemes:\n  - type: http\n    scheme: bearer\n    description: Bearer token in Authorization header.\n  - type: apiKey\n    in: header\n    name: X-API-Key\n    description: API key passed in X-API-Key header.\n"
source_yaml_url: https://artifacts.apis.io/rendlet-com/authentication/rendlet-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- PDF
- API
- DocumentGeneration
- SaaS
- DeveloperFriendly
- AI
---
