---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openeo-account-management-api-openapi.yml
  format: yaml
  label: openEO Account Management API
  slug: openeo-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/openapi/openeo-account-management-api-openapi.yml
- filename: openeo-batch-jobs-api-openapi.yml
  format: yaml
  label: openEO Batch Jobs API
  slug: openeo-batch-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/openapi/openeo-batch-jobs-api-openapi.yml
- filename: openeo-capabilities-api-openapi.yml
  format: yaml
  label: openEO Capabilities API
  slug: openeo-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/openapi/openeo-capabilities-api-openapi.yml
- filename: openeo-data-processing-api-openapi.yml
  format: yaml
  label: openEO Data Processing API
  slug: openeo-data-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/openapi/openeo-data-processing-api-openapi.yml
- filename: openeo-eo-data-discovery-api-openapi.yml
  format: yaml
  label: openEO EO Data Discovery API
  slug: openeo-eo-data-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/openapi/openeo-eo-data-discovery-api-openapi.yml
- filename: openeo-file-storage-api-openapi.yml
  format: yaml
  label: openEO File Storage API
  slug: openeo-file-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/openapi/openeo-file-storage-api-openapi.yml
- filename: openeo-orders-api-openapi.yml
  format: yaml
  label: openEO Orders API
  slug: openeo-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/openapi/openeo-orders-api-openapi.yml
- filename: openeo-process-discovery-api-openapi.yml
  format: yaml
  label: openEO Process Discovery API
  slug: openeo-process-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/openapi/openeo-process-discovery-api-openapi.yml
- filename: openeo-secondary-services-api-openapi.yml
  format: yaml
  label: openEO Secondary Services API
  slug: openeo-secondary-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/openapi/openeo-secondary-services-api-openapi.yml
- filename: openeo-user-defined-processes-api-openapi.yml
  format: yaml
  label: openEO User-Defined Processes API
  slug: openeo-user-defined-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/openapi/openeo-user-defined-processes-api-openapi.yml
- filename: openeo-workspaces-api-openapi.yml
  format: yaml
  label: openEO Workspaces API
  slug: openeo-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/openapi/openeo-workspaces-api-openapi.yml
auth_types:
- http
- unknown
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Openeo Authentication
name_suffix: Authentication
oauth_flows: []
overview: openEO secures its APIs with http and unknown across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: openEO
provider_slug: openeo
scheme_count: 3
schemes:
- bearerFormat: 'The Bearer Token MUST consist of the authentication method, a provider ID (if available) and the token itself. All separated by a forward slash `/`. Examples (replace `TOKEN` with the actual access token): (1) Basic authentication (no provider ID available): `basic//TOKEN` (2) OpenID Connect (provider ID is `ms`): `oidc/ms/TOKEN`. For OpenID Connect, the provider ID corresponds to the value specified for `id` for each provider in `GET /credentials/oidc`.'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/openeo-commercial-data-openapi.yml
  - openapi/openeo-openapi.yml
  type: http
- name: Basic
  scheme: basic
  sources:
  - openapi/openeo-commercial-data-openapi.yml
  - openapi/openeo-openapi.yml
  type: http
- name: Bearer
  sources:
  - openapi/openeo-processing-parameters-openapi.yml
  - openapi/openeo-workspaces-openapi.yml
  type: unknown
slug: openeo-authentication
source_filename: openeo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: searched\nsource: https://openeo.org/documentation/1.0/authentication.html; openapi/openeo-commercial-data-openapi.yml, openapi/openeo-openapi.yml,\n  openapi/openeo-processing-parameters-openapi.yml, openapi/openeo-workspaces-openapi.yml\nsummary:\n  types:\n  - http\n  - unknown\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: 'The Bearer Token MUST consist of the authentication method, a provider ID (if available) and the\n    token itself. All separated by a forward slash `/`. Examples (replace `TOKEN` with the actual access token):\n    (1) Basic authentication (no provider ID available): `basic//TOKEN` (2) OpenID Connect (provider ID is `ms`):\n    `oidc/ms/TOKEN`. For OpenID Connect, the provider ID corresponds to the value specified for `id` for each provider\n    in `GET /credentials/oidc`.'\n  sources:\n  - openapi/openeo-commercial-data-openapi.yml\n  - openapi/openeo-openapi.yml\n- name: Basic\n  type: http\n\
  \  scheme: basic\n  sources:\n  - openapi/openeo-commercial-data-openapi.yml\n  - openapi/openeo-openapi.yml\n- name: Bearer\n  type: unknown\n  sources:\n  - openapi/openeo-processing-parameters-openapi.yml\n  - openapi/openeo-workspaces-openapi.yml\ndocs: https://openeo.org/documentation/1.0/authentication.html\ndocs_summary:\n  methods:\n  - OpenID Connect (recommended) - authorization code, device flow, refresh token flow; providers discovered via\n    GET /credentials/oidc\n  - HTTP Basic (not recommended) via GET /credentials/basic, returns a token\n  bearer_format: basic//TOKEN or oidc/<provider_id>/TOKEN (openEO-specific format deprecated in 1.3.0 in favour\n    of standard JWT)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/authentication/openeo-authentication.yml
summary_line: http/unknown · 3 schemes
tags:
- Company
- Earth Observation
- Geospatial
- Remote Sensing
- Cloud Processing
- Open Source
- API Specification
- Data Cubes
---
