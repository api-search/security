---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: fluvigil-de-flood-situation-api-openapi.yml
  format: yaml
  label: Fluvigil Flood Situation API
  slug: fluvigil-de-flood-situation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluvigil-de/openapi/fluvigil-de-flood-situation-api-openapi.yml
- filename: fluvigil-de-health-api-openapi.yml
  format: yaml
  label: Fluvigil Health API
  slug: fluvigil-de-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluvigil-de/openapi/fluvigil-de-health-api-openapi.yml
- filename: fluvigil-de-me-api-openapi.yml
  format: yaml
  label: Fluvigil Me API
  slug: fluvigil-de-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluvigil-de/openapi/fluvigil-de-me-api-openapi.yml
- filename: fluvigil-de-rivers-api-openapi.yml
  format: yaml
  label: Fluvigil Rivers API
  slug: fluvigil-de-rivers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluvigil-de/openapi/fluvigil-de-rivers-api-openapi.yml
- filename: fluvigil-de-sources-api-openapi.yml
  format: yaml
  label: Fluvigil Sources API
  slug: fluvigil-de-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluvigil-de/openapi/fluvigil-de-sources-api-openapi.yml
- filename: fluvigil-de-stations-api-openapi.yml
  format: yaml
  label: Fluvigil Stations API
  slug: fluvigil-de-stations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluvigil-de/openapi/fluvigil-de-stations-api-openapi.yml
- filename: fluvigil-de-stats-api-openapi.yml
  format: yaml
  label: Fluvigil Stats API
  slug: fluvigil-de-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluvigil-de/openapi/fluvigil-de-stats-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Fluvigil De Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fluvigil secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fluvigil
provider_slug: fluvigil-de
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/fluvigil-de-openapi.yaml
  type: apiKey
slug: fluvigil-de-authentication
source_filename: fluvigil-de-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/fluvigil-de-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/fluvigil-de-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/fluvigil-de/authentication/fluvigil-de-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Water
- Environment
- Data
- API
- Germany
---
