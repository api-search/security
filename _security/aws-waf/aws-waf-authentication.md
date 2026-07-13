---
api_key_in:
- header
api_specs:
- filename: aws-waf-openapi.yml
  format: yaml
  label: AWS WAFV2 API
  slug: wafv2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-waf/refs/heads/main/openapi/aws-waf-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aws Waf Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS WAF secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS WAF
provider_slug: aws-waf
scheme_count: 1
schemes:
- description: 'AWS Signature Version 4. The `Authorization` header carries the SigV4

    signature derived from your access key and secret. See

    https://docs.aws.amazon.com/general/latest/gr/signature-version-4.html.'
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/aws-waf-openapi.yml
  type: apiKey
slug: aws-waf-authentication
source_filename: aws-waf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-waf-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    AWS Signature Version 4. The `Authorization` header carries the SigV4\n    signature derived from your access key and secret. See\n    https://docs.aws.amazon.com/general/latest/gr/signature-version-4.html.\n  sources:\n  - openapi/aws-waf-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-waf/refs/heads/main/authentication/aws-waf-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Security
- Web Application Firewall
- DDoS Protection
- Bot Management
- Edge Security
- Cloud
---
