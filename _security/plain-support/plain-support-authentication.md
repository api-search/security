---
api_key_in: []
api_specs:
- filename: plain-support-openapi.yml
  format: yaml
  label: Plain Customers API
  slug: plain-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plain-support/refs/heads/main/openapi/plain-support-openapi.yml
- filename: plain-support-openapi.yml
  format: yaml
  label: Plain Threads API
  slug: plain-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plain-support/refs/heads/main/openapi/plain-support-openapi.yml
- filename: plain-support-openapi.yml
  format: yaml
  label: Plain Timeline & Events API
  slug: plain-timeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plain-support/refs/heads/main/openapi/plain-support-openapi.yml
- filename: plain-support-openapi.yml
  format: yaml
  label: Plain Messages API
  slug: plain-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plain-support/refs/heads/main/openapi/plain-support-openapi.yml
- filename: plain-support-openapi.yml
  format: yaml
  label: Plain Labels & Tiers API
  slug: plain-labels-tiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plain-support/refs/heads/main/openapi/plain-support-openapi.yml
- filename: plain-support-openapi.yml
  format: yaml
  label: Plain Webhooks API
  slug: plain-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plain-support/refs/heads/main/openapi/plain-support-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Plain Support Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plain secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Plain
provider_slug: plain-support
scheme_count: 1
schemes:
- description: 'Plain API key issued to a Machine User, sent as a Bearer token: `Authorization: Bearer [example key]`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/plain-support-openapi.yml
  type: http
slug: plain-support-authentication
source_filename: plain-support-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/plain-support-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Plain API key issued to a Machine User, sent as a Bearer token: `Authorization:\n    Bearer [example key]`.'\n  sources:\n  - openapi/plain-support-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plain-support/refs/heads/main/authentication/plain-support-authentication.yml
summary_line: http · 1 scheme
tags:
- Customer Support
- Help Desk
- GraphQL
- Threads
- Customer Communication
- API First
---
