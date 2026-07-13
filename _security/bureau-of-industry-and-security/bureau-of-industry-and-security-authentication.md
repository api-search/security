---
api_key_in:
- header
api_specs:
- filename: bureau-of-industry-and-security-openapi.yml
  format: yaml
  label: Consolidated Screening List (CSL) API
  slug: consolidated-screening-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-industry-and-security/refs/heads/main/openapi/bureau-of-industry-and-security-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bureau Of Industry And Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bureau of Industry and Security secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bureau of Industry and Security
provider_slug: bureau-of-industry-and-security
scheme_count: 1
schemes:
- description: Subscription key issued by developer.trade.gov
  in: header
  name: subscriptionKey
  parameter: subscription-key
  sources:
  - openapi/bureau-of-industry-and-security-openapi.yml
  type: apiKey
slug: bureau-of-industry-and-security-authentication
source_filename: bureau-of-industry-and-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bureau-of-industry-and-security-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: subscriptionKey\n  type: apiKey\n  in: header\n  parameter: subscription-key\n  description: Subscription key issued by developer.trade.gov\n  sources:\n  - openapi/bureau-of-industry-and-security-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-industry-and-security/refs/heads/main/authentication/bureau-of-industry-and-security-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Compliance
- Export Controls
- Federal Government
- Industries
- National Security
- Screening Lists
- Security
---
