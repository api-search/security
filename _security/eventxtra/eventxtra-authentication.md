---
api_key_in:
- header
api_specs:
- filename: eventxtra-attendee-api-openapi.yml
  format: yaml
  label: EventX Attendee API
  slug: eventxtra-attendee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-attendee-api-openapi.yml
- filename: eventxtra-auth-api-openapi.yml
  format: yaml
  label: EventX Auth API
  slug: eventxtra-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-auth-api-openapi.yml
- filename: eventxtra-custom-field-api-openapi.yml
  format: yaml
  label: EventX Custom Field API
  slug: eventxtra-custom-field-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-custom-field-api-openapi.yml
- filename: eventxtra-event-api-openapi.yml
  format: yaml
  label: EventX Event API
  slug: eventxtra-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-event-api-openapi.yml
- filename: eventxtra-event-webhook-api-openapi.yml
  format: yaml
  label: EventX Event Webhook API
  slug: eventxtra-event-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-event-webhook-api-openapi.yml
- filename: eventxtra-invoice-api-openapi.yml
  format: yaml
  label: EventX Invoice API
  slug: eventxtra-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-invoice-api-openapi.yml
- filename: eventxtra-media-api-openapi.yml
  format: yaml
  label: EventX Media API
  slug: eventxtra-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-media-api-openapi.yml
- filename: eventxtra-order-api-openapi.yml
  format: yaml
  label: EventX Order API
  slug: eventxtra-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-order-api-openapi.yml
- filename: eventxtra-outreach-api-openapi.yml
  format: yaml
  label: EventX Outreach API
  slug: eventxtra-outreach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-outreach-api-openapi.yml
- filename: eventxtra-public-api-api-openapi.yml
  format: yaml
  label: EventX Public API
  slug: eventxtra-public-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-public-api-api-openapi.yml
- filename: eventxtra-registration-form-api-openapi.yml
  format: yaml
  label: EventX Registration Form API
  slug: eventxtra-registration-form-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-registration-form-api-openapi.yml
- filename: eventxtra-registration-order-api-openapi.yml
  format: yaml
  label: EventX Registration Order API
  slug: eventxtra-registration-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-registration-order-api-openapi.yml
- filename: eventxtra-registration-service-api-openapi.yml
  format: yaml
  label: EventX Registration Service API
  slug: eventxtra-registration-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-registration-service-api-openapi.yml
- filename: eventxtra-salesforce-api-openapi.yml
  format: yaml
  label: EventX Salesforce API
  slug: eventxtra-salesforce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-salesforce-api-openapi.yml
- filename: eventxtra-ticket-class-api-openapi.yml
  format: yaml
  label: EventX Ticket Class API
  slug: eventxtra-ticket-class-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-ticket-class-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Eventxtra Authentication
name_suffix: Authentication
oauth_flows: []
overview: EventX secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: EventX
provider_slug: eventxtra
scheme_count: 1
schemes:
- description: Bearer Authorization with jwt token
  in: header
  name: bearerAuth
  parameter: Authorization
  sources:
  - openapi/eventxtra-public-api-openapi.json
  type: apiKey
slug: eventxtra-authentication
source_filename: eventxtra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/eventxtra-public-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Bearer Authorization with jwt token\n  sources:\n  - openapi/eventxtra-public-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/authentication/eventxtra-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Event Management
- Event Registration
- Ticketing
- Check-in
- Event Marketing
- Virtual Events
- Webhook
- OpenAPI
- MCP
- Artificial Intelligence
- Hong Kong
- APAC
---
