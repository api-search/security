---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: AWS Service Catalog API
  slug: aws-service-catalog-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/servicecatalog/2015-12-10/openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Service Catalog Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Service Catalog secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Service Catalog
provider_slug: amazon-service-catalog
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: AWSSignatureV4
  parameter: Authorization
  sources:
  - openapi/amazon-service-catalog-openapi.yml
  type: apiKey
slug: amazon-service-catalog-authentication
source_filename: amazon-service-catalog-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-service-catalog-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AWSSignatureV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-service-catalog-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-service-catalog/refs/heads/main/authentication/amazon-service-catalog-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Governance
- Compliance
- IT Governance
- Service Catalog
---
