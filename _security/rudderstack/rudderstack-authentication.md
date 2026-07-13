---
api_key_in: []
api_specs:
- filename: rudderstack-gateway-openapi.yml
  format: yaml
  label: RudderStack HTTP Tracking API
  slug: rudderstack-http-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rudderstack/refs/heads/main/openapi/rudderstack-gateway-openapi.yml
- filename: rudderstack-event-streaming-asyncapi.yml
  format: yaml
  label: RudderStack Webhook Source API
  slug: rudderstack-webhook-source-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/rudderstack/refs/heads/main/asyncapi/rudderstack-event-streaming-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rudderstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: RudderStack secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RudderStack
provider_slug: rudderstack
scheme_count: 1
schemes:
- description: Write Key Basic Authentication
  name: writeKeyAuth
  scheme: basic
  sources:
  - openapi/rudderstack-gateway-openapi.yml
  type: http
slug: rudderstack-authentication
source_filename: rudderstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rudderstack-gateway-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: writeKeyAuth\n  type: http\n  scheme: basic\n  description: Write Key Basic Authentication\n  sources:\n  - openapi/rudderstack-gateway-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rudderstack/refs/heads/main/authentication/rudderstack-authentication.yml
summary_line: http · 1 scheme
tags:
- Customer Data Platform
- CDP
- Data Pipeline
- Open Source
- Event Streaming
- Reverse ETL
- Analytics
- Identity Resolution
---
