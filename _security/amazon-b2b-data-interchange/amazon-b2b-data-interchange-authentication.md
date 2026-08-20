---
api_key_in:
- header
api_specs:
- filename: amazon-b2b-data-interchange-capabilities-api-openapi.yml
  format: yaml
  label: Amazon B2B Data Interchange Capabilities API
  slug: amazon-b2b-data-interchange-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-b2b-data-interchange/refs/heads/main/openapi/amazon-b2b-data-interchange-capabilities-api-openapi.yml
- filename: amazon-b2b-data-interchange-partnerships-api-openapi.yml
  format: yaml
  label: Amazon B2B Data Interchange Partnerships API
  slug: amazon-b2b-data-interchange-partnerships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-b2b-data-interchange/refs/heads/main/openapi/amazon-b2b-data-interchange-partnerships-api-openapi.yml
- filename: amazon-b2b-data-interchange-profiles-api-openapi.yml
  format: yaml
  label: Amazon B2B Data Interchange Profiles API
  slug: amazon-b2b-data-interchange-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-b2b-data-interchange/refs/heads/main/openapi/amazon-b2b-data-interchange-profiles-api-openapi.yml
- filename: amazon-b2b-data-interchange-tags-api-openapi.yml
  format: yaml
  label: Amazon B2B Data Interchange Tags API
  slug: amazon-b2b-data-interchange-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-b2b-data-interchange/refs/heads/main/openapi/amazon-b2b-data-interchange-tags-api-openapi.yml
- filename: amazon-b2b-data-interchange-testing-api-openapi.yml
  format: yaml
  label: Amazon B2B Data Interchange Testing API
  slug: amazon-b2b-data-interchange-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-b2b-data-interchange/refs/heads/main/openapi/amazon-b2b-data-interchange-testing-api-openapi.yml
- filename: amazon-b2b-data-interchange-transformers-api-openapi.yml
  format: yaml
  label: Amazon B2B Data Interchange Transformers API
  slug: amazon-b2b-data-interchange-transformers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-b2b-data-interchange/refs/heads/main/openapi/amazon-b2b-data-interchange-transformers-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon B2B Data Interchange Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon B2B Data Interchange secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon B2B Data Interchange
provider_slug: amazon-b2b-data-interchange
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: aws_iam
  parameter: Authorization
  sources:
  - openapi/aws-b2b-data-interchange-api-openapi.yml
  type: apiKey
slug: amazon-b2b-data-interchange-authentication
source_filename: amazon-b2b-data-interchange-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-b2b-data-interchange-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_iam\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/aws-b2b-data-interchange-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-b2b-data-interchange/refs/heads/main/authentication/amazon-b2b-data-interchange-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- EDI
- B2B
- Data Interchange
- Supply Chain
- Healthcare
- Financial-Services
- Amazon Web Services
---
