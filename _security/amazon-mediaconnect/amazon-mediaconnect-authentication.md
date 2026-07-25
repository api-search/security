---
api_key_in:
- header
api_specs:
- filename: amazon-mediaconnect-bridges-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Bridges API
  slug: amazon-mediaconnect-bridges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/openapi/amazon-mediaconnect-bridges-api-openapi.yml
- filename: amazon-mediaconnect-entitlements-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Entitlements API
  slug: amazon-mediaconnect-entitlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/openapi/amazon-mediaconnect-entitlements-api-openapi.yml
- filename: amazon-mediaconnect-flows-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Flows API
  slug: amazon-mediaconnect-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/openapi/amazon-mediaconnect-flows-api-openapi.yml
- filename: amazon-mediaconnect-gateway-instances-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Gateway Instances API
  slug: amazon-mediaconnect-gateway-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/openapi/amazon-mediaconnect-gateway-instances-api-openapi.yml
- filename: amazon-mediaconnect-gateways-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Gateways API
  slug: amazon-mediaconnect-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/openapi/amazon-mediaconnect-gateways-api-openapi.yml
- filename: amazon-mediaconnect-offerings-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Offerings API
  slug: amazon-mediaconnect-offerings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/openapi/amazon-mediaconnect-offerings-api-openapi.yml
- filename: amazon-mediaconnect-reservations-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Reservations API
  slug: amazon-mediaconnect-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/openapi/amazon-mediaconnect-reservations-api-openapi.yml
- filename: amazon-mediaconnect-tags-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Tags API
  slug: amazon-mediaconnect-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/openapi/amazon-mediaconnect-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Mediaconnect Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon MediaConnect secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-mediaconnect-openapi-original.yml
  type: apiKey
slug: amazon-mediaconnect-authentication
source_filename: amazon-mediaconnect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-mediaconnect-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-mediaconnect-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/authentication/amazon-mediaconnect-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
---
