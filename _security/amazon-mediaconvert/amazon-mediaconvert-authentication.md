---
api_key_in:
- header
api_specs:
- filename: amazon-mediaconvert-certificates-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert Certificates API
  slug: amazon-mediaconvert-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-certificates-api-openapi.yml
- filename: amazon-mediaconvert-endpoints-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert Endpoints API
  slug: amazon-mediaconvert-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-endpoints-api-openapi.yml
- filename: amazon-mediaconvert-jobs-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert Jobs API
  slug: amazon-mediaconvert-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-jobs-api-openapi.yml
- filename: amazon-mediaconvert-jobtemplates-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert JobTemplates API
  slug: amazon-mediaconvert-jobtemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-jobtemplates-api-openapi.yml
- filename: amazon-mediaconvert-policy-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert Policy API
  slug: amazon-mediaconvert-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-policy-api-openapi.yml
- filename: amazon-mediaconvert-presets-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert Presets API
  slug: amazon-mediaconvert-presets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-presets-api-openapi.yml
- filename: amazon-mediaconvert-queues-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert Queues API
  slug: amazon-mediaconvert-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-queues-api-openapi.yml
- filename: amazon-mediaconvert-tags-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert Tags API
  slug: amazon-mediaconvert-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Mediaconvert Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon MediaConvert secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-mediaconvert-openapi-original.yml
  type: apiKey
slug: amazon-mediaconvert-authentication
source_filename: amazon-mediaconvert-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-mediaconvert-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-mediaconvert-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/authentication/amazon-mediaconvert-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Broadcasting
- Media Processing
- Media
---
