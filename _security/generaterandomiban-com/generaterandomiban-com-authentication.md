---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: generaterandomiban-com-countries-api-openapi.yml
  format: yaml
  label: Random IBAN Generator Countries API
  slug: generaterandomiban-com-countries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/generaterandomiban-com/openapi/generaterandomiban-com-countries-api-openapi.yml
- filename: generaterandomiban-com-generation-api-openapi.yml
  format: yaml
  label: Random IBAN Generator Generation API
  slug: generaterandomiban-com-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/generaterandomiban-com/openapi/generaterandomiban-com-generation-api-openapi.yml
- filename: generaterandomiban-com-service-api-openapi.yml
  format: yaml
  label: Random IBAN Generator Service API
  slug: generaterandomiban-com-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/generaterandomiban-com/openapi/generaterandomiban-com-service-api-openapi.yml
- filename: generaterandomiban-com-validation-api-openapi.yml
  format: yaml
  label: Random IBAN Generator Validation API
  slug: generaterandomiban-com-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/generaterandomiban-com/openapi/generaterandomiban-com-validation-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Random IBAN Generator Authentication
name_suffix: Authentication
oauth_flows: []
overview: Random IBAN Generator secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Random IBAN Generator
provider_slug: generaterandomiban-com
scheme_count: 1
schemes:
- description: 'API key issued on request. Send it in the X-API-Key header (an Authorization: Bearer token also works). Request a key by email at apis@generaterandomiban.com.'
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/generaterandomiban-com-openapi.json
  type: apiKey
slug: generaterandomiban-com-authentication
source_filename: generaterandomiban-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/generaterandomiban-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'API key issued on request. Send it in the X-API-Key header (an Authorization:\n    Bearer token also works). Request a key by email at apis@generaterandomiban.com.'\n  sources:\n  - openapi/generaterandomiban-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/generaterandomiban-com/authentication/generaterandomiban-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Finance
- Testing
- Utilities
- Open Source
---
