---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fence-authentication-api-openapi.yml
  format: yaml
  label: Fence Authentication API
  slug: fence-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fence/openapi/fence-authentication-api-openapi.yml
- filename: fence-declaration-monitoring-api-openapi.yml
  format: yaml
  label: Fence Declaration monitoring API
  slug: fence-declaration-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fence/openapi/fence-declaration-monitoring-api-openapi.yml
- filename: fence-documents-api-openapi.yml
  format: yaml
  label: Fence Documents API
  slug: fence-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fence/openapi/fence-documents-api-openapi.yml
- filename: fence-payments-api-openapi.yml
  format: yaml
  label: Fence Payments API
  slug: fence-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fence/openapi/fence-payments-api-openapi.yml
- filename: fence-portfolio-declarations-api-openapi.yml
  format: yaml
  label: Fence Portfolio declarations API
  slug: fence-portfolio-declarations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fence/openapi/fence-portfolio-declarations-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fence Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fence declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Fence
provider_slug: fence
scheme_count: 1
schemes:
- flow: clientCredentials
  scopes: {}
  tokenUrl: https://dev-api.fence.finance/v1/login/access-token
  type: oauth2
slug: fence-authentication
source_filename: fence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://docs.fence.finance/#authentication\nschemes:\n  - type: oauth2\n    flow: clientCredentials\n    tokenUrl: https://dev-api.fence.finance/v1/login/access-token\n    scopes: {}\n"
source_yaml_url: https://artifacts.apis.io/fence/authentication/fence-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Fintech
- Asset-Backed-Finance
- Real-Time
- API
---
