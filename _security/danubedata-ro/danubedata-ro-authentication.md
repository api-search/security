---
anonymous_access: false
api_key_in: []
api_specs:
- filename: danubedata-ro-openapi-generated.yml
  format: yaml
  label: Danube Data API
  slug: danubedata-ro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/danubedata-ro/openapi/_ae-authored/danubedata-ro-openapi-generated.yml
auth_types: []
description: Authentication methods documented for Danube Data APIs and serverless containers.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Danubedata Ro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Danube Data declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Danube Data
provider_slug: danubedata-ro
scheme_count: 1
schemes:
- evidence: All DanubeData API requests require authentication using Laravel Sanctum bearer tokens.
  header: Authorization
  how_to_obtain: Create an API token in the Security → API tokens page of the DanubeData console; the token is shown once and must be copied and stored securely.
  location: header
  name: Bearer
  type: http-bearer
slug: danubedata-ro-authentication
source_filename: danubedata-ro-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.danubedata.ro/api-authentication
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.danubedata.ro/api-authentication\nsources:\n- https://docs.danubedata.ro/api-authentication\n- https://docs.danubedata.ro/serverless-authentication\n- https://docs.danubedata.ro/getting-started\n- https://docs.danubedata.ro/quick-start\ndescription: Authentication methods documented for Danube Data APIs and serverless containers.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: All DanubeData API requests require authentication using Laravel Sanctum bearer tokens.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API token in the Security → API tokens page of the DanubeData console; the token is shown once and must be copied and\n    stored securely.\ndocs: https://docs.danubedata.ro/api-authentication\nnote: 4 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/danubedata-ro/authentication/danubedata-ro-authentication.yml
summary_line: 1 scheme
tags:
- Cloud
- Virtual Machines
- Managed Database
- Object Storage
- Serverless
- Kubernetes
- Caching
- Developer Tools
---
