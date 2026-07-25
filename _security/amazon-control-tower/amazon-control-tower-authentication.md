---
api_key_in: []
api_specs:
- filename: amazon-control-tower-baselines-api-openapi.yml
  format: yaml
  label: Amazon Control Tower Baselines API
  slug: amazon-control-tower-baselines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/openapi/amazon-control-tower-baselines-api-openapi.yml
- filename: amazon-control-tower-controls-api-openapi.yml
  format: yaml
  label: Amazon Control Tower Controls API
  slug: amazon-control-tower-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/openapi/amazon-control-tower-controls-api-openapi.yml
- filename: amazon-control-tower-landing-zones-api-openapi.yml
  format: yaml
  label: Amazon Control Tower Landing Zones API
  slug: amazon-control-tower-landing-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/openapi/amazon-control-tower-landing-zones-api-openapi.yml
- filename: amazon-control-tower-tags-api-openapi.yml
  format: yaml
  label: Amazon Control Tower Tags API
  slug: amazon-control-tower-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/openapi/amazon-control-tower-tags-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Control Tower Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Control Tower secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication. Requests must be signed using IAM credentials with appropriate AWS Control Tower permissions.
  name: aws_signature
  scheme: bearer
  sources:
  - openapi/amazon-control-tower-openapi.yml
  type: http
slug: amazon-control-tower-authentication
source_filename: amazon-control-tower-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-control-tower-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: aws_signature\n  type: http\n  scheme: bearer\n  description: AWS Signature Version 4 authentication. Requests must be signed using IAM credentials\n    with appropriate AWS Control Tower permissions.\n  sources:\n  - openapi/amazon-control-tower-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/authentication/amazon-control-tower-authentication.yml
summary_line: http · 1 scheme
tags:
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
---
