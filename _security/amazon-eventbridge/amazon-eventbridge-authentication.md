---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-eventbridge-archives-api-openapi.yml
  format: yaml
  label: Amazon EventBridge Archives API
  slug: amazon-eventbridge-archives-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eventbridge/openapi/amazon-eventbridge-archives-api-openapi.yml
- filename: amazon-eventbridge-event-buses-api-openapi.yml
  format: yaml
  label: Amazon EventBridge Event Buses API
  slug: amazon-eventbridge-event-buses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eventbridge/openapi/amazon-eventbridge-event-buses-api-openapi.yml
- filename: amazon-eventbridge-events-api-openapi.yml
  format: yaml
  label: Amazon EventBridge Events API
  slug: amazon-eventbridge-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eventbridge/openapi/amazon-eventbridge-events-api-openapi.yml
- filename: amazon-eventbridge-rules-api-openapi.yml
  format: yaml
  label: Amazon EventBridge Rules API
  slug: amazon-eventbridge-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eventbridge/openapi/amazon-eventbridge-rules-api-openapi.yml
- filename: amazon-eventbridge-targets-api-openapi.yml
  format: yaml
  label: Amazon EventBridge Targets API
  slug: amazon-eventbridge-targets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eventbridge/openapi/amazon-eventbridge-targets-api-openapi.yml
- filename: amazon-eventbridge-api-destination-api-openapi.yml
  format: yaml
  label: Amazon EventBridge Eventbridge Api Destination API
  slug: amazon-eventbridge-api-destination-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eventbridge/openapi/amazon-eventbridge-api-destination-api-openapi.yml
- filename: amazon-eventbridge-connection-api-openapi.yml
  format: yaml
  label: Amazon EventBridge Eventbridge Connection API
  slug: amazon-eventbridge-connection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eventbridge/openapi/amazon-eventbridge-connection-api-openapi.yml
- filename: amazon-eventbridge-endpoint-api-openapi.yml
  format: yaml
  label: Amazon EventBridge Eventbridge Endpoint API
  slug: amazon-eventbridge-endpoint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eventbridge/openapi/amazon-eventbridge-endpoint-api-openapi.yml
- filename: amazon-eventbridge-event-bus-api-openapi.yml
  format: yaml
  label: Amazon EventBridge Eventbridge Event Bus API
  slug: amazon-eventbridge-event-bus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eventbridge/openapi/amazon-eventbridge-event-bus-api-openapi.yml
- filename: amazon-eventbridge-operations-api-openapi.yml
  format: yaml
  label: Amazon EventBridge Eventbridge Operations API
  slug: amazon-eventbridge-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eventbridge/openapi/amazon-eventbridge-operations-api-openapi.yml
- filename: amazon-eventbridge-partner-event-source-api-openapi.yml
  format: yaml
  label: Amazon EventBridge Eventbridge Partner Event Source API
  slug: amazon-eventbridge-partner-event-source-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eventbridge/openapi/amazon-eventbridge-partner-event-source-api-openapi.yml
- filename: amazon-eventbridge-replay-api-openapi.yml
  format: yaml
  label: Amazon EventBridge Eventbridge Replay API
  slug: amazon-eventbridge-replay-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eventbridge/openapi/amazon-eventbridge-replay-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Eventbridge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon EventBridge secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon EventBridge
provider_slug: amazon-eventbridge
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication.
  in: header
  name: aws_sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-eventbridge-openapi.yml
  type: apiKey
slug: amazon-eventbridge-authentication
source_filename: amazon-eventbridge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-eventbridge-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication.\n  sources:\n  - openapi/amazon-eventbridge-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-eventbridge/authentication/amazon-eventbridge-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Event Bus
- Event-Driven
- Event
- Integration
- Serverless
---
