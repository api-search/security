---
api_key_in:
- query
api_specs:
- filename: shopper-approved-openapi.yml
  format: yaml
  label: Shopper Approved API
  slug: shopper-approved-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopper-approved/refs/heads/main/openapi/shopper-approved-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Shopper Approved Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shopper Approved secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shopper Approved
provider_slug: shopper-approved
scheme_count: 1
schemes:
- description: Shopper Approved API token (used with site_id path parameter)
  in: query
  name: SiteIdToken
  parameter: token
  sources:
  - openapi/shopper-approved-openapi.yml
  type: apiKey
slug: shopper-approved-authentication
source_filename: shopper-approved-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shopper-approved-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: SiteIdToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: Shopper Approved API token (used with site_id path parameter)\n  sources:\n  - openapi/shopper-approved-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopper-approved/refs/heads/main/authentication/shopper-approved-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Reviews
- Ratings
- Ecommerce
- Customer Feedback
- Social Proof
---
