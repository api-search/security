---
api_key_in:
- header
api_specs:
- filename: amazon-monitron-projectadmins-api-openapi.yml
  format: yaml
  label: Amazon Monitron ProjectAdmins API
  slug: amazon-monitron-projectadmins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-monitron/refs/heads/main/openapi/amazon-monitron-projectadmins-api-openapi.yml
- filename: amazon-monitron-projects-api-openapi.yml
  format: yaml
  label: Amazon Monitron Projects API
  slug: amazon-monitron-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-monitron/refs/heads/main/openapi/amazon-monitron-projects-api-openapi.yml
- filename: amazon-monitron-tags-api-openapi.yml
  format: yaml
  label: Amazon Monitron Tags API
  slug: amazon-monitron-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-monitron/refs/heads/main/openapi/amazon-monitron-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Monitron Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Monitron secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Monitron
provider_slug: amazon-monitron
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: awsSigV4
  parameter: Authorization
  sources:
  - openapi/amazon-monitron-openapi-original.yml
  type: apiKey
slug: amazon-monitron-authentication
source_filename: amazon-monitron-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-monitron-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: awsSigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-monitron-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-monitron/refs/heads/main/authentication/amazon-monitron-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Broadcasting
- Media Processing
- Media
---
