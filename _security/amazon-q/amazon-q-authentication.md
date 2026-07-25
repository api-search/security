---
api_key_in:
- header
api_specs:
- filename: amazon-q-applications-api-openapi.yml
  format: yaml
  label: Amazon Q Applications API
  slug: amazon-q-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-q/refs/heads/main/openapi/amazon-q-applications-api-openapi.yml
- filename: amazon-q-conversations-api-openapi.yml
  format: yaml
  label: Amazon Q Conversations API
  slug: amazon-q-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-q/refs/heads/main/openapi/amazon-q-conversations-api-openapi.yml
- filename: amazon-q-data-sources-api-openapi.yml
  format: yaml
  label: Amazon Q Data Sources API
  slug: amazon-q-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-q/refs/heads/main/openapi/amazon-q-data-sources-api-openapi.yml
- filename: amazon-q-indices-api-openapi.yml
  format: yaml
  label: Amazon Q Indices API
  slug: amazon-q-indices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-q/refs/heads/main/openapi/amazon-q-indices-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Q Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Q secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Q
provider_slug: amazon-q
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-q-openapi.yml
  type: apiKey
slug: amazon-q-authentication
source_filename: amazon-q-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-q-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-q-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-q/refs/heads/main/authentication/amazon-q-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Assistant
- Enterprise
- Generative AI
---
