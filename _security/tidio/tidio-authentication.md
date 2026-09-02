---
api_key_in:
- header
api_specs:
- filename: tidio-contacts-api-openapi.yml
  format: yaml
  label: Tidio Contacts API
  slug: tidio-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidio/refs/heads/main/openapi/tidio-contacts-api-openapi.yml
- filename: tidio-departments-api-openapi.yml
  format: yaml
  label: Tidio Departments API
  slug: tidio-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidio/refs/heads/main/openapi/tidio-departments-api-openapi.yml
- filename: tidio-lyro-api-openapi.yml
  format: yaml
  label: Tidio Lyro API
  slug: tidio-lyro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidio/refs/heads/main/openapi/tidio-lyro-api-openapi.yml
- filename: tidio-operators-api-openapi.yml
  format: yaml
  label: Tidio Operators API
  slug: tidio-operators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidio/refs/heads/main/openapi/tidio-operators-api-openapi.yml
- filename: tidio-products-api-openapi.yml
  format: yaml
  label: Tidio Products API
  slug: tidio-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidio/refs/heads/main/openapi/tidio-products-api-openapi.yml
- filename: tidio-project-api-openapi.yml
  format: yaml
  label: Tidio Project API
  slug: tidio-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidio/refs/heads/main/openapi/tidio-project-api-openapi.yml
- filename: tidio-tickets-api-openapi.yml
  format: yaml
  label: Tidio Tickets API
  slug: tidio-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidio/refs/heads/main/openapi/tidio-tickets-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tidio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tidio secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tidio
provider_slug: tidio
scheme_count: 2
schemes:
- in: header
  name: clientId
  parameter: X-Tidio-Openapi-Client-Id
  sources:
  - openapi/tidio-openapi-openapi.yml
  type: apiKey
- in: header
  name: clientSecret
  parameter: X-Tidio-Openapi-Client-Secret
  sources:
  - openapi/tidio-openapi-openapi.yml
  type: apiKey
slug: tidio-authentication
source_filename: tidio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tidio-openapi-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: clientId\n  type: apiKey\n  in: header\n  parameter: X-Tidio-Openapi-Client-Id\n  sources:\n  - openapi/tidio-openapi-openapi.yml\n- name: clientSecret\n  type: apiKey\n  in: header\n  parameter: X-Tidio-Openapi-Client-Secret\n  sources:\n  - openapi/tidio-openapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tidio/refs/heads/main/authentication/tidio-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Live Chat
- Chatbots
- Customer Service
- Artificial Intelligence
- Help Desk
- Ticketing
- Conversations
- Contacts
- Webhook
- Widget
---
