---
api_key_in:
- header
api_specs:
- filename: aws-marketplace-change-sets-api-openapi.yml
  format: yaml
  label: AWS Marketplace Change Sets API
  slug: aws-marketplace-change-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-marketplace/refs/heads/main/openapi/aws-marketplace-change-sets-api-openapi.yml
- filename: aws-marketplace-entities-api-openapi.yml
  format: yaml
  label: AWS Marketplace Entities API
  slug: aws-marketplace-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-marketplace/refs/heads/main/openapi/aws-marketplace-entities-api-openapi.yml
- filename: aws-marketplace-resource-policies-api-openapi.yml
  format: yaml
  label: AWS Marketplace Resource Policies API
  slug: aws-marketplace-resource-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-marketplace/refs/heads/main/openapi/aws-marketplace-resource-policies-api-openapi.yml
- filename: aws-marketplace-tags-api-openapi.yml
  format: yaml
  label: AWS Marketplace Tags API
  slug: aws-marketplace-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-marketplace/refs/heads/main/openapi/aws-marketplace-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aws Marketplace Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS Marketplace secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS Marketplace
provider_slug: aws-marketplace
scheme_count: 1
schemes:
- description: AWS Signature Version 4 signed Authorization header
  in: header
  name: SigV4
  parameter: Authorization
  sources:
  - openapi/aws-marketplace-openapi.yml
  type: apiKey
slug: aws-marketplace-authentication
source_filename: aws-marketplace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-marketplace-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 signed Authorization header\n  sources:\n  - openapi/aws-marketplace-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-marketplace/refs/heads/main/authentication/aws-marketplace-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Marketplace
- Procurement
- Software-as-a-Service
- Software Distribution
- Catalog
---
