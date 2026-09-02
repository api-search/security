---
api_key_in: []
api_specs:
- filename: dolby-io-abr-ladders-api-openapi.yml
  format: yaml
  label: Dolby.io ABR Ladders API
  slug: dolby-io-abr-ladders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-abr-ladders-api-openapi.yml
- filename: dolby-io-analytics-api-openapi.yml
  format: yaml
  label: Dolby.io Analytics API
  slug: dolby-io-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-analytics-api-openapi.yml
- filename: dolby-io-channels-api-openapi.yml
  format: yaml
  label: Dolby.io Channels API
  slug: dolby-io-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-channels-api-openapi.yml
- filename: dolby-io-cluster-api-openapi.yml
  format: yaml
  label: Dolby.io Cluster API
  slug: dolby-io-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-cluster-api-openapi.yml
- filename: dolby-io-custom-endpoint-providers-api-openapi.yml
  format: yaml
  label: Dolby.io Custom Endpoint Providers API
  slug: dolby-io-custom-endpoint-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-custom-endpoint-providers-api-openapi.yml
- filename: dolby-io-custom-endpoints-api-openapi.yml
  format: yaml
  label: Dolby.io Custom Endpoints API
  slug: dolby-io-custom-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-custom-endpoints-api-openapi.yml
- filename: dolby-io-distributions-api-openapi.yml
  format: yaml
  label: Dolby.io Distributions API
  slug: dolby-io-distributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-distributions-api-openapi.yml
- filename: dolby-io-engines-api-openapi.yml
  format: yaml
  label: Dolby.io Engines API
  slug: dolby-io-engines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-engines-api-openapi.yml
- filename: dolby-io-ingests-api-openapi.yml
  format: yaml
  label: Dolby.io Ingests API
  slug: dolby-io-ingests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-ingests-api-openapi.yml
- filename: dolby-io-publishtoken-api-openapi.yml
  format: yaml
  label: Dolby.io PublishToken API
  slug: dolby-io-publishtoken-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-publishtoken-api-openapi.yml
- filename: dolby-io-regions-api-openapi.yml
  format: yaml
  label: Dolby.io Regions API
  slug: dolby-io-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-regions-api-openapi.yml
- filename: dolby-io-subscribetoken-api-openapi.yml
  format: yaml
  label: Dolby.io SubscribeToken API
  slug: dolby-io-subscribetoken-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-subscribetoken-api-openapi.yml
- filename: dolby-io-webhook-api-openapi.yml
  format: yaml
  label: Dolby.io Webhook API
  slug: dolby-io-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-webhook-api-openapi.yml
- filename: dolby-io-webhooks-api-openapi.yml
  format: yaml
  label: Dolby.io Webhooks API
  slug: dolby-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dolby Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dolby.io secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dolby.io
provider_slug: dolby-io
scheme_count: 2
schemes:
- bearerFormat: API Secret
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/dolby-io-realtime-streaming-api-openapi.yml
  type: http
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/dolby-io-theolive-api-openapi.yml
  type: http
slug: dolby-io-authentication
source_filename: dolby-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dolby-io-realtime-streaming-api-openapi.yml, openapi/dolby-io-theolive-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Secret\n  sources:\n  - openapi/dolby-io-realtime-streaming-api-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/dolby-io-theolive-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/authentication/dolby-io-authentication.yml
summary_line: http · 2 schemes
tags:
- Media
- Streaming
- Real-Time Streaming
- WebRTC
- Live Streaming
- Low Latency
- Video
- Audio
- Broadcast
- Player
- Advertising
- Dolby OptiView
- Millicast
- THEOlive
- THEOplayer
---
