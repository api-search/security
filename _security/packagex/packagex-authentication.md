---
api_key_in:
- header
api_specs:
- filename: packagex-openapi-original.yml
  format: yaml
  label: PackageX Shipments API
  slug: packagex-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/packagex/refs/heads/main/openapi/packagex-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Packagex Authentication
name_suffix: Authentication
oauth_flows: []
overview: PackageX secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PackageX
provider_slug: packagex
scheme_count: 1
schemes:
- alt_parameter: X-API-KEY
  in: header
  name: api_key
  parameter: PX-API-KEY
  sources:
  - openapi/packagex-openapi-original.yml
  type: apiKey
slug: packagex-authentication
source_filename: packagex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/packagex-openapi-original.yml\ndocs: https://docs.packagex.io/apis/getting-started/authenication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nnotes: >-\n  PackageX uses API-key authentication passed in a request header. Keys are\n  generated in the PackageX Dashboard, separately for the Sandbox and Production\n  environments; an \"owner\" or \"developer\" account role is required to create\n  them. Keys are shown only once and cannot be recovered if lost. All requests\n  must be made over HTTPS; plain HTTP and unauthenticated requests fail. API\n  keys can be scoped to restrict access to only the APIs they need.\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: PX-API-KEY\n  alt_parameter: X-API-KEY\n  sources:\n  - openapi/packagex-openapi-original.yml\nenvironments:\n- name: production\n  base_url: https://api.packagex.io\n- name: sandbox\n  base_url: https://sandbox--api.packagex.io\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/packagex/refs/heads/main/authentication/packagex-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Logistics
- Shipping
- Supply Chain
- Computer Vision
- OCR
- Package Tracking
- Fulfillment
---
