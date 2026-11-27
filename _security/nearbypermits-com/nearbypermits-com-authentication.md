---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: nearbypermits-com-address-api-openapi.yml
  format: yaml
  label: Nearby Permits Address API
  slug: nearbypermits-com-address-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nearbypermits-com/openapi/nearbypermits-com-address-api-openapi.yml
- filename: nearbypermits-com-cities-api-openapi.yml
  format: yaml
  label: Nearby Permits Cities API
  slug: nearbypermits-com-cities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nearbypermits-com/openapi/nearbypermits-com-cities-api-openapi.yml
- filename: nearbypermits-com-near-api-openapi.yml
  format: yaml
  label: Nearby Permits Near API
  slug: nearbypermits-com-near-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nearbypermits-com/openapi/nearbypermits-com-near-api-openapi.yml
- filename: nearbypermits-com-permit-api-openapi.yml
  format: yaml
  label: Nearby Permits Permit API
  slug: nearbypermits-com-permit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nearbypermits-com/openapi/nearbypermits-com-permit-api-openapi.yml
- filename: nearbypermits-com-recent-api-openapi.yml
  format: yaml
  label: Nearby Permits Recent API
  slug: nearbypermits-com-recent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nearbypermits-com/openapi/nearbypermits-com-recent-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Nearby Permits Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nearby Permits secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nearby Permits
provider_slug: nearbypermits-com
scheme_count: 2
schemes:
- description: Free key from https://nearbypermits.com/developers/#key
  name: bearerKey
  scheme: bearer
  sources:
  - openapi/nearbypermits-com-openapi.json
  type: http
- in: query
  name: queryKey
  parameter: key
  sources:
  - openapi/nearbypermits-com-openapi.json
  type: apiKey
slug: nearbypermits-com-authentication
source_filename: nearbypermits-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/nearbypermits-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: bearerKey\n  type: http\n  scheme: bearer\n  description: Free key from https://nearbypermits.com/developers/#key\n  sources:\n  - openapi/nearbypermits-com-openapi.json\n- name: queryKey\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/nearbypermits-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/nearbypermits-com/authentication/nearbypermits-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Permits
- Construction
---
