---
api_key_in:
- header
api_specs:
- filename: amazon-outposts-openapi.yml
  format: yaml
  label: AWS Outposts API
  slug: aws-outposts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/openapi/amazon-outposts-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Outposts Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Outposts secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Outposts
provider_slug: amazon-outposts
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-outposts-openapi.yml
  type: apiKey
slug: amazon-outposts-authentication
source_filename: amazon-outposts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-outposts-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-outposts-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/authentication/amazon-outposts-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
---
