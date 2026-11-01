---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-entity-resolution-matchingworkflows-api-openapi.yml
  format: yaml
  label: Amazon Entity Resolution Matchingworkflows API
  slug: amazon-entity-resolution-matchingworkflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-entity-resolution/openapi/amazon-entity-resolution-matchingworkflows-api-openapi.yml
- filename: amazon-entity-resolution-schemas-api-openapi.yml
  format: yaml
  label: Amazon Entity Resolution Schemas API
  slug: amazon-entity-resolution-schemas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-entity-resolution/openapi/amazon-entity-resolution-schemas-api-openapi.yml
- filename: amazon-entity-resolution-tags-api-openapi.yml
  format: yaml
  label: Amazon Entity Resolution Tags API
  slug: amazon-entity-resolution-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-entity-resolution/openapi/amazon-entity-resolution-tags-api-openapi.yml
- filename: amazon-entity-resolution-idmappingworkflows-api-openapi.yml
  format: yaml
  label: Amazon Entity Resolution Entity Resolution Idmappingworkflows API
  slug: amazon-entity-resolution-idmappingworkflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-entity-resolution/openapi/amazon-entity-resolution-idmappingworkflows-api-openapi.yml
- filename: amazon-entity-resolution-idnamespaces-api-openapi.yml
  format: yaml
  label: Amazon Entity Resolution Entity Resolution Idnamespaces API
  slug: amazon-entity-resolution-idnamespaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-entity-resolution/openapi/amazon-entity-resolution-idnamespaces-api-openapi.yml
- filename: amazon-entity-resolution-jobs-api-openapi.yml
  format: yaml
  label: Amazon Entity Resolution Entity Resolution Jobs API
  slug: amazon-entity-resolution-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-entity-resolution/openapi/amazon-entity-resolution-jobs-api-openapi.yml
- filename: amazon-entity-resolution-operations-api-openapi.yml
  format: yaml
  label: Amazon Entity Resolution Entity Resolution Operations API
  slug: amazon-entity-resolution-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-entity-resolution/openapi/amazon-entity-resolution-operations-api-openapi.yml
- filename: amazon-entity-resolution-policies-api-openapi.yml
  format: yaml
  label: Amazon Entity Resolution Entity Resolution Policies API
  slug: amazon-entity-resolution-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-entity-resolution/openapi/amazon-entity-resolution-policies-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Entity Resolution Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Entity Resolution secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-entity-resolution-openapi.yml
  type: apiKey
slug: amazon-entity-resolution-authentication
source_filename: amazon-entity-resolution-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-entity-resolution-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-entity-resolution-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-entity-resolution/authentication/amazon-entity-resolution-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
---
