---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hamburg-de-access-data-api-openapi.yml
  format: yaml
  label: Freie und Hansestadt Hamburg Access data API
  slug: hamburg-de-access-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hamburg-de/openapi/hamburg-de-access-data-api-openapi.yml
- filename: hamburg-de-capabilities-api-openapi.yml
  format: yaml
  label: Freie und Hansestadt Hamburg Capabilities API
  slug: hamburg-de-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hamburg-de/openapi/hamburg-de-capabilities-api-openapi.yml
- filename: hamburg-de-discover-data-collections-api-openapi.yml
  format: yaml
  label: Freie und Hansestadt Hamburg Discover data collections API
  slug: hamburg-de-discover-data-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hamburg-de/openapi/hamburg-de-discover-data-collections-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Freie und Hansestadt Hamburg Authentication
name_suffix: Authentication
oauth_flows: []
overview: Freie und Hansestadt Hamburg secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Freie und Hansestadt Hamburg
provider_slug: hamburg-de
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: Default
  scheme: bearer
  sources:
  - openapi/hamburg-de-badegewaesser-openapi.yml
  - openapi/hamburg-de-baustellen-openapi.yml
  - openapi/hamburg-de-bplaene-openapi.yml
  - openapi/hamburg-de-denkmalschutz-openapi.yml
  - openapi/hamburg-de-emobility-openapi.yml
  type: http
slug: hamburg-de-authentication
source_filename: hamburg-de-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/hamburg-de-badegewaesser-openapi.yml, openapi/hamburg-de-baustellen-openapi.yml,\n  openapi/hamburg-de-bplaene-openapi.yml, openapi/hamburg-de-denkmalschutz-openapi.yml, openapi/hamburg-de-emobility-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: Default\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/hamburg-de-badegewaesser-openapi.yml\n  - openapi/hamburg-de-baustellen-openapi.yml\n  - openapi/hamburg-de-bplaene-openapi.yml\n  - openapi/hamburg-de-denkmalschutz-openapi.yml\n  - openapi/hamburg-de-emobility-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/hamburg-de/authentication/hamburg-de-authentication.yml
summary_line: http · 1 scheme
tags:
- Government
- Open Data
- Geospatial
- OGC API Features
- Smart City
- Germany
- Urban Data Platform
---
