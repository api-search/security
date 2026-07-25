---
api_key_in:
- header
api_specs:
- filename: bunny-net-stream-webhooks-asyncapi.yml
  format: yaml
  label: Bunny.net Stream Webhooks
  slug: stream-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunny-net/refs/heads/main/asyncapi/bunny-net-stream-webhooks-asyncapi.yml
- filename: bunny-net-apikeys-api-openapi.yml
  format: yaml
  label: Bunny.net APIKeys API
  slug: bunny-net-apikeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunny-net/refs/heads/main/openapi/bunny-net-apikeys-api-openapi.yml
- filename: bunny-net-billing-api-openapi.yml
  format: yaml
  label: Bunny.net Billing API
  slug: bunny-net-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunny-net/refs/heads/main/openapi/bunny-net-billing-api-openapi.yml
- filename: bunny-net-countries-api-openapi.yml
  format: yaml
  label: Bunny.net Countries API
  slug: bunny-net-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunny-net/refs/heads/main/openapi/bunny-net-countries-api-openapi.yml
- filename: bunny-net-dnszones-api-openapi.yml
  format: yaml
  label: Bunny.net DNSZones API
  slug: bunny-net-dnszones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunny-net/refs/heads/main/openapi/bunny-net-dnszones-api-openapi.yml
- filename: bunny-net-pullzones-api-openapi.yml
  format: yaml
  label: Bunny.net PullZones API
  slug: bunny-net-pullzones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunny-net/refs/heads/main/openapi/bunny-net-pullzones-api-openapi.yml
- filename: bunny-net-purge-api-openapi.yml
  format: yaml
  label: Bunny.net Purge API
  slug: bunny-net-purge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunny-net/refs/heads/main/openapi/bunny-net-purge-api-openapi.yml
- filename: bunny-net-regions-api-openapi.yml
  format: yaml
  label: Bunny.net Regions API
  slug: bunny-net-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunny-net/refs/heads/main/openapi/bunny-net-regions-api-openapi.yml
- filename: bunny-net-statistics-api-openapi.yml
  format: yaml
  label: Bunny.net Statistics API
  slug: bunny-net-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunny-net/refs/heads/main/openapi/bunny-net-statistics-api-openapi.yml
- filename: bunny-net-storagezones-api-openapi.yml
  format: yaml
  label: Bunny.net StorageZones API
  slug: bunny-net-storagezones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunny-net/refs/heads/main/openapi/bunny-net-storagezones-api-openapi.yml
- filename: bunny-net-stream-api-openapi.yml
  format: yaml
  label: Bunny.net Stream API
  slug: bunny-net-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunny-net/refs/heads/main/openapi/bunny-net-stream-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bunny Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bunny.net secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bunny.net
provider_slug: bunny-net
scheme_count: 1
schemes:
- description: API key issued from the Bunny.net dashboard.
  in: header
  name: accessKeyAuth
  parameter: AccessKey
  sources:
  - openapi/bunny-net-openapi.yml
  type: apiKey
slug: bunny-net-authentication
source_filename: bunny-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bunny-net-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: accessKeyAuth\n  type: apiKey\n  in: header\n  parameter: AccessKey\n  description: API key issued from the Bunny.net dashboard.\n  sources:\n  - openapi/bunny-net-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bunny-net/refs/heads/main/authentication/bunny-net-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CDN
- Edge
- Video
- Storage
- DNS
- WAF
- Edge Compute
- Image Optimization
---
