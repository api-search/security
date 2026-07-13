---
api_key_in: []
api_specs:
- filename: svix-openapi.json
  format: json
  label: Svix Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-openapi.json
- filename: svix-openapi.json
  format: json
  label: Svix Ingest API
  slug: ingest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-openapi.json
- filename: svix-openapi.json
  format: json
  label: Svix Stream API
  slug: stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-openapi.json
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
  - openapi/svix-openapi.json
  type: http
slug: svix-authentication
source_filename: svix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/svix-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  description: HTTP Bearer token passed in the `Authorization` header\n  sources:\n  - openapi/svix-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/authentication/svix-authentication.yml
summary_line: http · 1 scheme
tags:
- Webhooks
- Webhooks As A Service
- Webhook Delivery
- Webhook Sending
- Event Driven
- Eventing
- Messaging
- Pub Sub
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
- Multi Tenant
- Multi Region
- Enterprise
- SaaS
- Developer Platform
- API
- REST
- SOC 2
- HIPAA
- PCI DSS
- GDPR
- Open Source
- Rust
- Polyglot SDK
- Terraform
- CLI
---
