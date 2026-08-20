---
api_key_in: []
api_specs:
- filename: intercom-admins-api-openapi.yml
  format: yaml
  label: Intercom Admins API
  slug: intercom-admins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intercom/refs/heads/main/openapi/intercom-admins-api-openapi.yml
- filename: intercom-articles-api-openapi.yml
  format: yaml
  label: Intercom Articles API
  slug: intercom-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intercom/refs/heads/main/openapi/intercom-articles-api-openapi.yml
- filename: intercom-companies-api-openapi.yml
  format: yaml
  label: Intercom Companies API
  slug: intercom-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intercom/refs/heads/main/openapi/intercom-companies-api-openapi.yml
- filename: intercom-contacts-api-openapi.yml
  format: yaml
  label: Intercom Contacts API
  slug: intercom-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intercom/refs/heads/main/openapi/intercom-contacts-api-openapi.yml
- filename: intercom-conversations-api-openapi.yml
  format: yaml
  label: Intercom Conversations API
  slug: intercom-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intercom/refs/heads/main/openapi/intercom-conversations-api-openapi.yml
- filename: intercom-data-events-api-openapi.yml
  format: yaml
  label: Intercom Data Events API
  slug: intercom-data-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intercom/refs/heads/main/openapi/intercom-data-events-api-openapi.yml
- filename: intercom-messages-api-openapi.yml
  format: yaml
  label: Intercom Messages API
  slug: intercom-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intercom/refs/heads/main/openapi/intercom-messages-api-openapi.yml
- filename: intercom-news-api-openapi.yml
  format: yaml
  label: Intercom News API
  slug: intercom-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intercom/refs/heads/main/openapi/intercom-news-api-openapi.yml
- filename: intercom-segments-api-openapi.yml
  format: yaml
  label: Intercom Segments API
  slug: intercom-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intercom/refs/heads/main/openapi/intercom-segments-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Intercom Authentication
name_suffix: Authentication
oauth_flows: []
overview: Intercom secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Intercom
provider_slug: intercom
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/intercom-openapi.yml
  type: http
slug: intercom-authentication
source_filename: intercom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/intercom-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/intercom-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intercom/refs/heads/main/authentication/intercom-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Customer Service
- Customer-Support
- Messaging
---
