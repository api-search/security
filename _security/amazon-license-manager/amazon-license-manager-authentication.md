---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-license-manager-license-configurations-api-openapi.yml
  format: yaml
  label: Amazon License Manager License Configurations API
  slug: amazon-license-manager-license-configurations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-license-manager/openapi/amazon-license-manager-license-configurations-api-openapi.yml
- filename: amazon-license-manager-grant-api-openapi.yml
  format: yaml
  label: Amazon License Manager License Manager Grant API
  slug: amazon-license-manager-grant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-license-manager/openapi/amazon-license-manager-grant-api-openapi.yml
- filename: amazon-license-manager-license-api-openapi.yml
  format: yaml
  label: Amazon License Manager License Manager License API
  slug: amazon-license-manager-license-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-license-manager/openapi/amazon-license-manager-license-api-openapi.yml
- filename: amazon-license-manager-license-asset-group-api-openapi.yml
  format: yaml
  label: Amazon License Manager License Manager License Asset Group API
  slug: amazon-license-manager-license-asset-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-license-manager/openapi/amazon-license-manager-license-asset-group-api-openapi.yml
- filename: amazon-license-manager-license-asset-ruleset-api-openapi.yml
  format: yaml
  label: Amazon License Manager License Manager License Asset Ruleset API
  slug: amazon-license-manager-license-asset-ruleset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-license-manager/openapi/amazon-license-manager-license-asset-ruleset-api-openapi.yml
- filename: amazon-license-manager-license-conversion-task-api-openapi.yml
  format: yaml
  label: Amazon License Manager License Manager License Conversion Task API
  slug: amazon-license-manager-license-conversion-task-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-license-manager/openapi/amazon-license-manager-license-conversion-task-api-openapi.yml
- filename: amazon-license-manager-license-manager-report-generator-api-openapi.yml
  format: yaml
  label: Amazon License Manager License Manager License Manager Report Generator API
  slug: amazon-license-manager-license-manager-report-generator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-license-manager/openapi/amazon-license-manager-license-manager-report-generator-api-openapi.yml
- filename: amazon-license-manager-operations-api-openapi.yml
  format: yaml
  label: Amazon License Manager License Manager Operations API
  slug: amazon-license-manager-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-license-manager/openapi/amazon-license-manager-operations-api-openapi.yml
- filename: amazon-license-manager-token-api-openapi.yml
  format: yaml
  label: Amazon License Manager License Manager Token API
  slug: amazon-license-manager-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-license-manager/openapi/amazon-license-manager-token-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon License Manager Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon License Manager secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon License Manager
provider_slug: amazon-license-manager
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-license-manager-openapi.yml
  type: apiKey
slug: amazon-license-manager-authentication
source_filename: amazon-license-manager-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-license-manager-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-license-manager-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-license-manager/authentication/amazon-license-manager-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Compliance
- Cost Management
- License Management
- Software Licensing
---
