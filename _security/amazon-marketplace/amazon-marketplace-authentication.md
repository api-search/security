---
api_key_in:
- header
api_specs:
- filename: amazon-marketplace-openapi-original.yaml
  format: yaml
  label: AWS Marketplace Catalog API
  slug: aws-marketplace-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-openapi-original.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Marketplace Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Marketplace secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-marketplace-openapi-original.yaml
  type: apiKey
slug: amazon-marketplace-authentication
source_filename: amazon-marketplace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-marketplace-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-marketplace-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/authentication/amazon-marketplace-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Commerce
- ISV
- Marketplace
- Software Catalog
---
