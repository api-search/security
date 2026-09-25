---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-codeguru-security-findings-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Security Findings API
  slug: amazon-codeguru-security-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/openapi/amazon-codeguru-security-findings-api-openapi.yml
- filename: amazon-codeguru-security-metrics-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Security Metrics API
  slug: amazon-codeguru-security-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/openapi/amazon-codeguru-security-metrics-api-openapi.yml
- filename: amazon-codeguru-security-scans-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Security Scans API
  slug: amazon-codeguru-security-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/openapi/amazon-codeguru-security-scans-api-openapi.yml
- filename: amazon-codeguru-security-tags-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Security Tags API
  slug: amazon-codeguru-security-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/openapi/amazon-codeguru-security-tags-api-openapi.yml
- filename: amazon-codeguru-security-account-configuration-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Security Account Configuration API
  slug: amazon-codeguru-security-account-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/openapi/amazon-codeguru-security-account-configuration-api-openapi.yml
- filename: amazon-codeguru-security-batch-get-findings-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Security Batch Get Findings API
  slug: amazon-codeguru-security-batch-get-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/openapi/amazon-codeguru-security-batch-get-findings-api-openapi.yml
- filename: amazon-codeguru-security-update-account-configuration-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Security Update Account Configuration API
  slug: amazon-codeguru-security-update-account-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/openapi/amazon-codeguru-security-update-account-configuration-api-openapi.yml
- filename: amazon-codeguru-security-upload-url-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Security Upload URL API
  slug: amazon-codeguru-security-upload-url-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/openapi/amazon-codeguru-security-upload-url-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Codeguru Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon CodeGuru Security secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-codeguru-security-openapi-original.yaml
  type: apiKey
slug: amazon-codeguru-security-authentication
source_filename: amazon-codeguru-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-codeguru-security-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-codeguru-security-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/authentication/amazon-codeguru-security-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
- Defunct
---
