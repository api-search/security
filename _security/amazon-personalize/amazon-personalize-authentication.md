---
api_key_in:
- header
api_specs:
- filename: API_Reference.html
  format: yaml
  label: Amazon Personalize API
  slug: amazon-personalize-api
  spec_type: OpenAPI
  url: https://docs.aws.amazon.com/personalize/latest/dg/API_Reference.html
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Personalize Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Personalize secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Personalize
provider_slug: amazon-personalize
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-personalize-openapi.yml
  type: apiKey
slug: amazon-personalize-authentication
source_filename: amazon-personalize-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-personalize-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-personalize-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-personalize/refs/heads/main/authentication/amazon-personalize-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Customer Experience
- Machine Learning
- ML
- Personalization
- Recommendations
---
