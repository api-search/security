---
api_key_in:
- header
api_specs:
- filename: amazon-mediapackage-channels-api-openapi.yml
  format: yaml
  label: Amazon MediaPackage Channels API
  slug: amazon-mediapackage-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/openapi/amazon-mediapackage-channels-api-openapi.yml
- filename: amazon-mediapackage-harvest-jobs-api-openapi.yml
  format: yaml
  label: Amazon MediaPackage Harvest Jobs API
  slug: amazon-mediapackage-harvest-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/openapi/amazon-mediapackage-harvest-jobs-api-openapi.yml
- filename: amazon-mediapackage-origin-endpoints-api-openapi.yml
  format: yaml
  label: Amazon MediaPackage Origin Endpoints API
  slug: amazon-mediapackage-origin-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/openapi/amazon-mediapackage-origin-endpoints-api-openapi.yml
- filename: amazon-mediapackage-tags-api-openapi.yml
  format: yaml
  label: Amazon MediaPackage Tags API
  slug: amazon-mediapackage-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/openapi/amazon-mediapackage-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Mediapackage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon MediaPackage secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-mediapackage-openapi-original.yml
  type: apiKey
slug: amazon-mediapackage-authentication
source_filename: amazon-mediapackage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-mediapackage-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-mediapackage-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/authentication/amazon-mediapackage-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Broadcasting
- Media Processing
- Media
---
