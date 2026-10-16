---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chloris-geospatial-aoi-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Aoi API
  slug: chloris-geospatial-aoi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-aoi-api-openapi.yml
- filename: chloris-geospatial-boundary-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Boundary API
  slug: chloris-geospatial-boundary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-boundary-api-openapi.yml
- filename: chloris-geospatial-collection-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Collection API
  slug: chloris-geospatial-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-collection-api-openapi.yml
- filename: chloris-geospatial-info-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Info API
  slug: chloris-geospatial-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-info-api-openapi.yml
- filename: chloris-geospatial-invite-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Invite API
  slug: chloris-geospatial-invite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-invite-api-openapi.yml
- filename: chloris-geospatial-mgrstiles-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Mgrs Tiles API
  slug: chloris-geospatial-mgrstiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-mgrstiles-api-openapi.yml
- filename: chloris-geospatial-organization-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Organization API
  slug: chloris-geospatial-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-organization-api-openapi.yml
- filename: chloris-geospatial-reportingunit-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Reporting Unit API
  slug: chloris-geospatial-reportingunit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-reportingunit-api-openapi.yml
- filename: chloris-geospatial-user-api-openapi.yml
  format: yaml
  label: Chloris Geospatial User API
  slug: chloris-geospatial-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-user-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Chloris Geospatial Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chloris Geospatial secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chloris Geospatial
provider_slug: chloris-geospatial
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/chloris-geospatial-openapi.yml
  type: http
slug: chloris-geospatial-authentication
source_filename: chloris-geospatial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: derived\nsource: openapi/chloris-geospatial-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/chloris-geospatial-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/authentication/chloris-geospatial-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Geospatial
- Carbon
- Data
- Environmental
---
