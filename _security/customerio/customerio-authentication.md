---
api_key_in: []
api_specs:
- filename: customerio-broadcasts-api-openapi.yml
  format: yaml
  label: Customer.io Broadcasts API
  slug: customerio-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-broadcasts-api-openapi.yml
- filename: customerio-campaigns-api-openapi.yml
  format: yaml
  label: Customer.io Campaigns API
  slug: customerio-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-campaigns-api-openapi.yml
- filename: customerio-collections-api-openapi.yml
  format: yaml
  label: Customer.io Collections API
  slug: customerio-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-collections-api-openapi.yml
- filename: customerio-customers-api-openapi.yml
  format: yaml
  label: Customer.io Customers API
  slug: customerio-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-customers-api-openapi.yml
- filename: customerio-devices-api-openapi.yml
  format: yaml
  label: Customer.io Devices API
  slug: customerio-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-devices-api-openapi.yml
- filename: customerio-events-api-openapi.yml
  format: yaml
  label: Customer.io Events API
  slug: customerio-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-events-api-openapi.yml
- filename: customerio-exports-api-openapi.yml
  format: yaml
  label: Customer.io Exports API
  slug: customerio-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-exports-api-openapi.yml
- filename: customerio-messages-api-openapi.yml
  format: yaml
  label: Customer.io Messages API
  slug: customerio-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-messages-api-openapi.yml
- filename: customerio-people-api-openapi.yml
  format: yaml
  label: Customer.io People API
  slug: customerio-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-people-api-openapi.yml
- filename: customerio-pipelines-api-openapi.yml
  format: yaml
  label: Customer.io Pipelines API
  slug: customerio-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-pipelines-api-openapi.yml
- filename: customerio-segments-api-openapi.yml
  format: yaml
  label: Customer.io Segments API
  slug: customerio-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-segments-api-openapi.yml
- filename: customerio-track-v2-api-openapi.yml
  format: yaml
  label: Customer.io Track v2 API
  slug: customerio-track-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-track-v2-api-openapi.yml
- filename: customerio-transactional-api-openapi.yml
  format: yaml
  label: Customer.io Transactional API
  slug: customerio-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-transactional-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Customerio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Customer.io secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Customer.io
provider_slug: customerio
scheme_count: 2
schemes:
- description: Track API auth. Base-64 encode site_id:api_key and pass it in the Authorization header (Basic ...).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/customerio-openapi.yml
  type: http
- description: App API and Pipelines API auth. Pass the App API key (or Pipelines source write key) as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/customerio-openapi.yml
  type: http
slug: customerio-authentication
source_filename: customerio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/customerio-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Track API auth. Base-64 encode site_id:api_key and pass it in the Authorization\n    header (Basic ...).\n  sources:\n  - openapi/customerio-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: App API and Pipelines API auth. Pass the App API key (or Pipelines source write\n    key) as a Bearer token in the Authorization header.\n  sources:\n  - openapi/customerio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/authentication/customerio-authentication.yml
summary_line: http · 2 schemes
tags:
- Customer Messaging
- Marketing Automation
- Email
- CDP
- Transactional
---
