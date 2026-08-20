---
api_key_in: []
api_specs:
- filename: augment-api-key-api-openapi.yml
  format: yaml
  label: Augment API Key API
  slug: augment-api-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augment/refs/heads/main/openapi/augment-api-key-api-openapi.yml
- filename: augment-carrier-management-api-openapi.yml
  format: yaml
  label: Augment Carrier Management API
  slug: augment-carrier-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augment/refs/heads/main/openapi/augment-carrier-management-api-openapi.yml
- filename: augment-carrier-support-api-openapi.yml
  format: yaml
  label: Augment Carrier Support API
  slug: augment-carrier-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augment/refs/heads/main/openapi/augment-carrier-support-api-openapi.yml
- filename: augment-load-management-api-openapi.yml
  format: yaml
  label: Augment Load Management API
  slug: augment-load-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augment/refs/heads/main/openapi/augment-load-management-api-openapi.yml
- filename: augment-webhook-endpoints-api-openapi.yml
  format: yaml
  label: Augment Webhook Endpoints API
  slug: augment-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augment/refs/heads/main/openapi/augment-webhook-endpoints-api-openapi.yml
- filename: augment-webhook-event-subscriptions-api-openapi.yml
  format: yaml
  label: Augment Webhook Event Subscriptions API
  slug: augment-webhook-event-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augment/refs/heads/main/openapi/augment-webhook-event-subscriptions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Augment Authentication
name_suffix: Authentication
oauth_flows: []
overview: Augment secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Augment
provider_slug: augment
scheme_count: 1
schemes:
- description: Authenticate with HTTP Basic auth by sending an empty username and your API key as the password, equivalent to encoding :<API_KEY> in the Basic credential.
  name: httpBasic
  scheme: basic
  sources:
  - openapi/augment-openapi-original.json
  type: http
slug: augment-authentication
source_filename: augment-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/augment-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: httpBasic\n  type: http\n  scheme: basic\n  description: Authenticate with HTTP Basic auth by sending an empty username and your API key\n    as the password, equivalent to encoding :<API_KEY> in the Basic credential.\n  sources:\n  - openapi/augment-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/augment/refs/heads/main/authentication/augment-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Logistics
- Freight
- Supply Chain
- Transportation
- Webhook
- Artificial Intelligence
- Automation
---
