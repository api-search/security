---
anonymous_access: false
api_key_in: []
api_specs:
- filename: opencrvs-org-attachments-api-openapi.yml
  format: yaml
  label: OpenCRVS Attachments API
  slug: opencrvs-org-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opencrvs-org/openapi/opencrvs-org-attachments-api-openapi.yml
- filename: opencrvs-org-events-api-openapi.yml
  format: yaml
  label: OpenCRVS Events API
  slug: opencrvs-org-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opencrvs-org/openapi/opencrvs-org-events-api-openapi.yml
- filename: opencrvs-org-integrations-api-openapi.yml
  format: yaml
  label: OpenCRVS Integrations API
  slug: opencrvs-org-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opencrvs-org/openapi/opencrvs-org-integrations-api-openapi.yml
- filename: opencrvs-org-locations-api-openapi.yml
  format: yaml
  label: OpenCRVS Locations API
  slug: opencrvs-org-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opencrvs-org/openapi/opencrvs-org-locations-api-openapi.yml
- filename: opencrvs-org-search-api-openapi.yml
  format: yaml
  label: OpenCRVS Search API
  slug: opencrvs-org-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opencrvs-org/openapi/opencrvs-org-search-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: OpenCRVS Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenCRVS secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenCRVS
provider_slug: opencrvs-org
scheme_count: 1
schemes:
- name: Authorization
  scheme: bearer
  sources:
  - openapi/events-openapi.yml
  type: http
slug: opencrvs-org-authentication
source_filename: opencrvs-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/events-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: Authorization\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/events-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/opencrvs-org/authentication/opencrvs-org-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Open Source
- CivilRegistration
- Government
---
