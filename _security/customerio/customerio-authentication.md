---
api_key_in: []
api_specs:
- filename: customerio-openapi.yml
  format: yaml
  label: Customer.io Track API
  slug: track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-openapi.yml
- filename: customerio-openapi.yml
  format: yaml
  label: Customer.io App / Transactional API
  slug: app-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-openapi.yml
- filename: customerio-openapi.yml
  format: yaml
  label: Customer.io Pipelines / Data Pipelines CDP API
  slug: pipelines-cdp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-openapi.yml
- filename: customerio-openapi.yml
  format: yaml
  label: Customer.io Reporting API
  slug: reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-openapi.yml
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
