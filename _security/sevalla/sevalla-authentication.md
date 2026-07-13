---
api_key_in: []
api_specs:
- filename: sevalla-openapi.yml
  format: yaml
  label: Sevalla Applications API
  slug: sevalla-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevalla/refs/heads/main/openapi/sevalla-openapi.yml
- filename: sevalla-openapi.yml
  format: yaml
  label: Sevalla Deployments API
  slug: sevalla-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevalla/refs/heads/main/openapi/sevalla-openapi.yml
- filename: sevalla-openapi.yml
  format: yaml
  label: Sevalla Databases API
  slug: sevalla-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevalla/refs/heads/main/openapi/sevalla-openapi.yml
- filename: sevalla-openapi.yml
  format: yaml
  label: Sevalla Static Sites API
  slug: sevalla-static-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevalla/refs/heads/main/openapi/sevalla-openapi.yml
- filename: sevalla-openapi.yml
  format: yaml
  label: Sevalla Object Storage API
  slug: sevalla-object-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevalla/refs/heads/main/openapi/sevalla-openapi.yml
- filename: sevalla-openapi.yml
  format: yaml
  label: Sevalla Pipelines API
  slug: sevalla-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevalla/refs/heads/main/openapi/sevalla-openapi.yml
- filename: sevalla-openapi.yml
  format: yaml
  label: Sevalla Operations API
  slug: sevalla-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevalla/refs/heads/main/openapi/sevalla-openapi.yml
- filename: sevalla-openapi.yml
  format: yaml
  label: Sevalla Company and Account API
  slug: sevalla-company-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevalla/refs/heads/main/openapi/sevalla-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sevalla Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sevalla secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sevalla
provider_slug: sevalla
scheme_count: 1
schemes:
- bearerFormat: apiToken
  description: Provide your Sevalla API token as a bearer token in the Authorization header. Create a token from the Sevalla dashboard; one token authenticates every endpoint.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sevalla-openapi.yml
  type: http
slug: sevalla-authentication
source_filename: sevalla-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sevalla-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: apiToken\n  description: Provide your Sevalla API token as a bearer token in the Authorization header.\n    Create a token from the Sevalla dashboard; one token authenticates every endpoint.\n  sources:\n  - openapi/sevalla-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sevalla/refs/heads/main/authentication/sevalla-authentication.yml
summary_line: http · 1 scheme
tags:
- Hosting
- PaaS
- Cloud
- Deployment
- Databases
- Static Sites
- Object Storage
---
