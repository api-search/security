---
api_key_in:
- header
api_specs:
- filename: amazon-codeguru-reviewer-associations-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Reviewer Associations API
  slug: amazon-codeguru-reviewer-associations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/openapi/amazon-codeguru-reviewer-associations-api-openapi.yml
- filename: amazon-codeguru-reviewer-codereviews-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Reviewer Codereviews API
  slug: amazon-codeguru-reviewer-codereviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/openapi/amazon-codeguru-reviewer-codereviews-api-openapi.yml
- filename: amazon-codeguru-reviewer-codereviews-type-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Reviewer Codereviews#Type API
  slug: amazon-codeguru-reviewer-codereviews-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/openapi/amazon-codeguru-reviewer-codereviews-type-api-openapi.yml
- filename: amazon-codeguru-reviewer-feedback-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Reviewer Feedback API
  slug: amazon-codeguru-reviewer-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/openapi/amazon-codeguru-reviewer-feedback-api-openapi.yml
- filename: amazon-codeguru-reviewer-tags-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Reviewer Tags API
  slug: amazon-codeguru-reviewer-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/openapi/amazon-codeguru-reviewer-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Codeguru Reviewer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon CodeGuru Reviewer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-codeguru-reviewer-openapi-original.yaml
  type: apiKey
slug: amazon-codeguru-reviewer-authentication
source_filename: amazon-codeguru-reviewer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-codeguru-reviewer-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-codeguru-reviewer-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/authentication/amazon-codeguru-reviewer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
---
