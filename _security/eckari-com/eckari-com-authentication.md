---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: eckari-com-company-information-api-openapi.yml
  format: yaml
  label: Eckari Company Information API
  slug: eckari-com-company-information-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eckari-com/openapi/eckari-com-company-information-api-openapi.yml
- filename: eckari-com-domain-intelligence-api-openapi.yml
  format: yaml
  label: Eckari Domain Intelligence API
  slug: eckari-com-domain-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eckari-com/openapi/eckari-com-domain-intelligence-api-openapi.yml
- filename: eckari-com-foreign-exchange-api-openapi.yml
  format: yaml
  label: Eckari Foreign Exchange API
  slug: eckari-com-foreign-exchange-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eckari-com/openapi/eckari-com-foreign-exchange-api-openapi.yml
- filename: eckari-com-location-api-openapi.yml
  format: yaml
  label: Eckari Location API
  slug: eckari-com-location-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eckari-com/openapi/eckari-com-location-api-openapi.yml
- filename: eckari-com-logistics-api-openapi.yml
  format: yaml
  label: Eckari Logistics API
  slug: eckari-com-logistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eckari-com/openapi/eckari-com-logistics-api-openapi.yml
- filename: eckari-com-weather-api-openapi.yml
  format: yaml
  label: Eckari Weather API
  slug: eckari-com-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eckari-com/openapi/eckari-com-weather-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Eckari Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eckari secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Eckari
provider_slug: eckari-com
scheme_count: 2
schemes:
- description: Eckari account API key (ek_test_… / ek_live_…) issued in the developer portal; usage is metered and billed in arrears.
  name: eckariApiKey
  scheme: bearer
  sources:
  - openapi/eckari-com-openapi.json
  type: http
- description: x402 accountless payment. An unpaid request receives HTTP 402 with a PAYMENT-REQUIRED header; retry with PAYMENT-SIGNATURE.
  in: header
  name: x402
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/eckari-com-openapi.json
  type: apiKey
slug: eckari-com-authentication
source_filename: eckari-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/eckari-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: eckariApiKey\n  type: http\n  scheme: bearer\n  description: Eckari account API key (ek_test_… / ek_live_…) issued in the developer portal;\n    usage is metered and billed in arrears.\n  sources:\n  - openapi/eckari-com-openapi.json\n- name: x402\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: x402 accountless payment. An unpaid request receives HTTP 402 with a PAYMENT-REQUIRED\n    header; retry with PAYMENT-SIGNATURE.\n  sources:\n  - openapi/eckari-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/eckari-com/authentication/eckari-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company Records
- Legal Entities
- Domain Data
- Weather
- Location
- Real-World Data
---
