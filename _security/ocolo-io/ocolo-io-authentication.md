---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: ocolo-io-guidance-api-openapi.yml
  format: yaml
  label: OCOLO Guidance API
  slug: ocolo-io-guidance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ocolo-io/openapi/ocolo-io-guidance-api-openapi.yml
- filename: ocolo-io-openapi-json-api-openapi.yml
  format: yaml
  label: OCOLO Openapi.json API
  slug: ocolo-io-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ocolo-io/openapi/ocolo-io-openapi-json-api-openapi.yml
- filename: ocolo-io-project-requests-api-openapi.yml
  format: yaml
  label: OCOLO Project Requests API
  slug: ocolo-io-project-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ocolo-io/openapi/ocolo-io-project-requests-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: OCOLO Authentication
name_suffix: Authentication
oauth_flows: []
overview: OCOLO secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OCOLO
provider_slug: ocolo-io
scheme_count: 2
schemes:
- description: The status_token returned when the request was created.
  name: statusToken
  scheme: bearer
  sources:
  - openapi/ocolo-io-openapi.json
  type: http
- description: Optional partner key; lifts rate limits and allows status reads without a token.
  in: header
  name: partnerApiKey
  parameter: X-Ocolo-Api-Key
  sources:
  - openapi/ocolo-io-openapi.json
  type: apiKey
slug: ocolo-io-authentication
source_filename: ocolo-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/ocolo-io-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: statusToken\n  type: http\n  scheme: bearer\n  description: The status_token returned when the request was created.\n  sources:\n  - openapi/ocolo-io-openapi.json\n- name: partnerApiKey\n  type: apiKey\n  in: header\n  parameter: X-Ocolo-Api-Key\n  description: Optional partner key; lifts rate limits and allows status reads without a token.\n  sources:\n  - openapi/ocolo-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/ocolo-io/authentication/ocolo-io-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Colocation
- Data Center Marketplace
- Enterprise IT
- Wholesale Capacity Data
- Ordering Portal Licensing
- Bid Management
---
