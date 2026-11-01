---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-shield-amazon-shield-rest-api-api-openapi.yml
  format: yaml
  label: Amazon Shield Amazon Shield REST API
  slug: amazon-shield-amazon-shield-rest-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-shield/openapi/amazon-shield-amazon-shield-rest-api-api-openapi.yml
- filename: amazon-shield-application-layer-automatic-response-api-openapi.yml
  format: yaml
  label: Amazon Shield Shield Application Layer Automatic Response API
  slug: amazon-shield-application-layer-automatic-response-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-shield/openapi/amazon-shield-application-layer-automatic-response-api-openapi.yml
- filename: amazon-shield-operations-api-openapi.yml
  format: yaml
  label: Amazon Shield Shield Operations API
  slug: amazon-shield-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-shield/openapi/amazon-shield-operations-api-openapi.yml
- filename: amazon-shield-protection-group-api-openapi.yml
  format: yaml
  label: Amazon Shield Shield Protection Group API
  slug: amazon-shield-protection-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-shield/openapi/amazon-shield-protection-group-api-openapi.yml
- filename: amazon-shield-resource-api-openapi.yml
  format: yaml
  label: Amazon Shield Shield Resource API
  slug: amazon-shield-resource-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-shield/openapi/amazon-shield-resource-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Shield Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Shield secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Shield
provider_slug: amazon-shield
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-shield-api-openapi.yml
  type: apiKey
slug: amazon-shield-authentication
source_filename: amazon-shield-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-shield-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-shield-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-shield/authentication/amazon-shield-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- DDoS Protection
- Networking
- Security
---
