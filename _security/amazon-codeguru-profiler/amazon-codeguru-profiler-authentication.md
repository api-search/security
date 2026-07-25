---
api_key_in:
- header
api_specs:
- filename: amazon-codeguru-profiler-internal-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Profiler Internal API
  slug: amazon-codeguru-profiler-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/openapi/amazon-codeguru-profiler-internal-api-openapi.yml
- filename: amazon-codeguru-profiler-profilinggroups-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Profiler ProfilingGroups API
  slug: amazon-codeguru-profiler-profilinggroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/openapi/amazon-codeguru-profiler-profilinggroups-api-openapi.yml
- filename: amazon-codeguru-profiler-profilinggroups-clienttoken-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Profiler ProfilingGroups#clientToken API
  slug: amazon-codeguru-profiler-profilinggroups-clienttoken-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/openapi/amazon-codeguru-profiler-profilinggroups-clienttoken-api-openapi.yml
- filename: amazon-codeguru-profiler-tags-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Profiler Tags API
  slug: amazon-codeguru-profiler-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/openapi/amazon-codeguru-profiler-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Codeguru Profiler Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon CodeGuru Profiler secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-codeguru-profiler-openapi-original.yaml
  type: apiKey
slug: amazon-codeguru-profiler-authentication
source_filename: amazon-codeguru-profiler-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-codeguru-profiler-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-codeguru-profiler-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/authentication/amazon-codeguru-profiler-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon
- Application Performance
- Profiling
- DevOps
- Machine Learning
---
