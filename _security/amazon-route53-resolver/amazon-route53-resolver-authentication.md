---
api_key_in:
- header
api_specs:
- filename: amazon-route53-resolver-openapi.yml
  format: yaml
  label: Amazon Route 53 Resolver API
  slug: amazon-route-53-resolver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/openapi/amazon-route53-resolver-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Route53 Resolver Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Route 53 Resolver secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-route53-resolver-openapi.yml
  type: apiKey
slug: amazon-route53-resolver-authentication
source_filename: amazon-route53-resolver-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-route53-resolver-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-route53-resolver-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/authentication/amazon-route53-resolver-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- DNS
- Hybrid Cloud
- Networking
---
