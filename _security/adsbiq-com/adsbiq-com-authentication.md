---
anonymous_access: false
api_key_in: []
api_specs:
- filename: adsbiq-com-aircraft-api-openapi.yml
  format: yaml
  label: adsbiq-com Aircraft API
  slug: adsbiq-com-aircraft-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsbiq-com/openapi/adsbiq-com-aircraft-api-openapi.yml
- filename: adsbiq-com-airports-api-openapi.yml
  format: yaml
  label: adsbiq-com Airports API
  slug: adsbiq-com-airports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsbiq-com/openapi/adsbiq-com-airports-api-openapi.yml
- filename: adsbiq-com-flights-api-openapi.yml
  format: yaml
  label: adsbiq-com Flights API
  slug: adsbiq-com-flights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsbiq-com/openapi/adsbiq-com-flights-api-openapi.yml
- filename: adsbiq-com-geographic-api-openapi.yml
  format: yaml
  label: adsbiq-com Geographic API
  slug: adsbiq-com-geographic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsbiq-com/openapi/adsbiq-com-geographic-api-openapi.yml
- filename: adsbiq-com-network-api-openapi.yml
  format: yaml
  label: adsbiq-com Network API
  slug: adsbiq-com-network-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsbiq-com/openapi/adsbiq-com-network-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Adsbiq Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: adsbiq-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: adsbiq-com
provider_slug: adsbiq-com
scheme_count: 1
schemes:
- bearerFormat: ADSBiq API key
  description: Feeder API key. Registered feeder IPs may also receive access without a header.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/adsbiq-com-openapi.yaml
  type: http
slug: adsbiq-com-authentication
source_filename: adsbiq-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/adsbiq-com-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: ADSBiq API key\n  description: Feeder API key. Registered feeder IPs may also receive access without a header.\n  sources:\n  - openapi/adsbiq-com-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/adsbiq-com/authentication/adsbiq-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Advertising
- DataAnalytics
- MarketingTechnology
- API
- Company
---
