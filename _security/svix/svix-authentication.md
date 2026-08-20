---
api_key_in: []
api_specs:
- filename: svix-application-api-openapi.yml
  format: yaml
  label: Svix Application API
  slug: svix-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-application-api-openapi.yml
- filename: svix-authentication-api-openapi.yml
  format: yaml
  label: Svix Authentication API
  slug: svix-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-authentication-api-openapi.yml
- filename: svix-background-task-api-openapi.yml
  format: yaml
  label: Svix Background Task API
  slug: svix-background-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-background-task-api-openapi.yml
- filename: svix-connector-api-openapi.yml
  format: yaml
  label: Svix Connector API
  slug: svix-connector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-connector-api-openapi.yml
- filename: svix-endpoint-api-openapi.yml
  format: yaml
  label: Svix Endpoint API
  slug: svix-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-endpoint-api-openapi.yml
- filename: svix-environment-api-openapi.yml
  format: yaml
  label: Svix Environment API
  slug: svix-environment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-environment-api-openapi.yml
- filename: svix-event-api-openapi.yml
  format: yaml
  label: Svix Event API
  slug: svix-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-event-api-openapi.yml
- filename: svix-event-type-api-openapi.yml
  format: yaml
  label: Svix Event Type API
  slug: svix-event-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-event-type-api-openapi.yml
- filename: svix-health-api-openapi.yml
  format: yaml
  label: Svix Health API
  slug: svix-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-health-api-openapi.yml
- filename: svix-ingest-endpoint-api-openapi.yml
  format: yaml
  label: Svix Ingest Endpoint API
  slug: svix-ingest-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-ingest-endpoint-api-openapi.yml
- filename: svix-ingest-source-api-openapi.yml
  format: yaml
  label: Svix Ingest Source API
  slug: svix-ingest-source-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-ingest-source-api-openapi.yml
- filename: svix-integration-api-openapi.yml
  format: yaml
  label: Svix Integration API
  slug: svix-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-integration-api-openapi.yml
- filename: svix-message-api-openapi.yml
  format: yaml
  label: Svix Message API
  slug: svix-message-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-message-api-openapi.yml
- filename: svix-message-attempt-api-openapi.yml
  format: yaml
  label: Svix Message Attempt API
  slug: svix-message-attempt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-message-attempt-api-openapi.yml
- filename: svix-sink-api-openapi.yml
  format: yaml
  label: Svix Sink API
  slug: svix-sink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-sink-api-openapi.yml
- filename: svix-statistics-api-openapi.yml
  format: yaml
  label: Svix Statistics API
  slug: svix-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-statistics-api-openapi.yml
- filename: svix-stream-api-openapi.yml
  format: yaml
  label: Svix Stream API
  slug: svix-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-stream-api-openapi.yml
- filename: svix-stream-authentication-api-openapi.yml
  format: yaml
  label: Svix Stream Authentication API
  slug: svix-stream-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-stream-authentication-api-openapi.yml
- filename: svix-stream-event-type-api-openapi.yml
  format: yaml
  label: Svix Stream Event Type API
  slug: svix-stream-event-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-stream-event-type-api-openapi.yml
- filename: svix-webhook-endpoint-api-openapi.yml
  format: yaml
  label: Svix Webhook Endpoint API
  slug: svix-webhook-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-webhook-endpoint-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Svix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Svix secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Svix
provider_slug: svix
scheme_count: 1
schemes:
- description: HTTP Bearer token passed in the `Authorization` header
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/svix-application-api-openapi.yml
  - openapi/svix-authentication-api-openapi.yml
  - openapi/svix-background-task-api-openapi.yml
  - openapi/svix-connector-api-openapi.yml
  - openapi/svix-endpoint-api-openapi.yml
  - openapi/svix-environment-api-openapi.yml
  - openapi/svix-event-api-openapi.yml
  - openapi/svix-event-type-api-openapi.yml
  - openapi/svix-health-api-openapi.yml
  - openapi/svix-ingest-endpoint-api-openapi.yml
  - openapi/svix-ingest-source-api-openapi.yml
  - openapi/svix-integration-api-openapi.yml
  - openapi/svix-message-api-openapi.yml
  - openapi/svix-message-attempt-api-openapi.yml
  - openapi/svix-sink-api-openapi.yml
  - openapi/svix-statistics-api-openapi.yml
  - openapi/svix-stream-api-openapi.yml
  - openapi/svix-stream-authentication-api-openapi.yml
  - openapi/svix-stream-event-type-api-openapi.yml
  - openapi/svix-webhook-endpoint-api-openapi.yml
  type: http
slug: svix-authentication
source_filename: svix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/svix-application-api-openapi.yml, openapi/svix-authentication-api-openapi.yml,\n  openapi/svix-background-task-api-openapi.yml, openapi/svix-connector-api-openapi.yml, openapi/svix-endpoint-api-openapi.yml,\n  openapi/svix-environment-api-openapi.yml, openapi/svix-event-api-openapi.yml, openapi/svix-event-type-api-openapi.yml,\n  openapi/svix-health-api-openapi.yml, openapi/svix-ingest-endpoint-api-openapi.yml, openapi/svix-ingest-source-api-openapi.yml,\n  openapi/svix-integration-api-openapi.yml ...\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  description: HTTP Bearer token passed in the `Authorization` header\n  sources:\n  - openapi/svix-application-api-openapi.yml\n  - openapi/svix-authentication-api-openapi.yml\n  - openapi/svix-background-task-api-openapi.yml\n  - openapi/svix-connector-api-openapi.yml\n  - openapi/svix-endpoint-api-openapi.yml\n  - openapi/svix-environment-api-openapi.yml\n\
  \  - openapi/svix-event-api-openapi.yml\n  - openapi/svix-event-type-api-openapi.yml\n  - openapi/svix-health-api-openapi.yml\n  - openapi/svix-ingest-endpoint-api-openapi.yml\n  - openapi/svix-ingest-source-api-openapi.yml\n  - openapi/svix-integration-api-openapi.yml\n  - openapi/svix-message-api-openapi.yml\n  - openapi/svix-message-attempt-api-openapi.yml\n  - openapi/svix-sink-api-openapi.yml\n  - openapi/svix-statistics-api-openapi.yml\n  - openapi/svix-stream-api-openapi.yml\n  - openapi/svix-stream-authentication-api-openapi.yml\n  - openapi/svix-stream-event-type-api-openapi.yml\n  - openapi/svix-webhook-endpoint-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/authentication/svix-authentication.yml
summary_line: http · 1 scheme
tags:
- Webhook
- Webhooks As A Service
- Webhook Delivery
- Webhook Sending
- Event-Driven
- Eventing
- Messaging
- Pub-Sub
- Streaming
- Ingest
- Integration
- Reliability
- Retries
- Deliverability
- Signing
- Verification
- HMAC
- Standard Webhooks
- Multi-Tenant
- Multi-Region
- Enterprise
- Software-as-a-Service
- Developer Platform
- REST
- SOC 2
- HIPAA
- PCI DSS
- GDPR
- Open-Source
- Rust
- Polyglot SDK
- Terraform
- CLI
---
