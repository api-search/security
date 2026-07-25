---
api_key_in: []
api_specs:
- filename: freshdesk-webhook-api-asyncapi.yml
  format: yaml
  label: Freshdesk Webhook API
  slug: webhook-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/asyncapi/freshdesk-webhook-api-asyncapi.yml
- filename: freshdesk-agents-api-openapi.yml
  format: yaml
  label: freshdesk Agents API
  slug: freshdesk-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-agents-api-openapi.yml
- filename: freshdesk-business-hours-api-openapi.yml
  format: yaml
  label: freshdesk Business Hours API
  slug: freshdesk-business-hours-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-business-hours-api-openapi.yml
- filename: freshdesk-companies-api-openapi.yml
  format: yaml
  label: freshdesk Companies API
  slug: freshdesk-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-companies-api-openapi.yml
- filename: freshdesk-contacts-api-openapi.yml
  format: yaml
  label: freshdesk Contacts API
  slug: freshdesk-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-contacts-api-openapi.yml
- filename: freshdesk-conversations-api-openapi.yml
  format: yaml
  label: freshdesk Conversations API
  slug: freshdesk-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-conversations-api-openapi.yml
- filename: freshdesk-email-configs-api-openapi.yml
  format: yaml
  label: freshdesk Email Configs API
  slug: freshdesk-email-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-email-configs-api-openapi.yml
- filename: freshdesk-groups-api-openapi.yml
  format: yaml
  label: freshdesk Groups API
  slug: freshdesk-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-groups-api-openapi.yml
- filename: freshdesk-products-api-openapi.yml
  format: yaml
  label: freshdesk Products API
  slug: freshdesk-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-products-api-openapi.yml
- filename: freshdesk-roles-api-openapi.yml
  format: yaml
  label: freshdesk Roles API
  slug: freshdesk-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-roles-api-openapi.yml
- filename: freshdesk-satisfaction-ratings-api-openapi.yml
  format: yaml
  label: freshdesk Satisfaction Ratings API
  slug: freshdesk-satisfaction-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-satisfaction-ratings-api-openapi.yml
- filename: freshdesk-search-api-openapi.yml
  format: yaml
  label: freshdesk Search API
  slug: freshdesk-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-search-api-openapi.yml
- filename: freshdesk-sla-policies-api-openapi.yml
  format: yaml
  label: freshdesk SLA Policies API
  slug: freshdesk-sla-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-sla-policies-api-openapi.yml
- filename: freshdesk-solutions-api-openapi.yml
  format: yaml
  label: freshdesk Solutions API
  slug: freshdesk-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-solutions-api-openapi.yml
- filename: freshdesk-tickets-api-openapi.yml
  format: yaml
  label: freshdesk Tickets API
  slug: freshdesk-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-tickets-api-openapi.yml
- filename: freshdesk-time-entries-api-openapi.yml
  format: yaml
  label: freshdesk Time Entries API
  slug: freshdesk-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-time-entries-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Freshdesk Authentication
name_suffix: Authentication
oauth_flows: []
overview: freshdesk secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: freshdesk
provider_slug: freshdesk
scheme_count: 1
schemes:
- description: Freshdesk uses API key-based authentication. Pass your API key as the username with any string (e.g. X) as the password using HTTP Basic Authentication.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/freshdesk-rest-api-openapi.yml
  type: http
slug: freshdesk-authentication
source_filename: freshdesk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/freshdesk-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Freshdesk uses API key-based authentication. Pass your API key as the username\n    with any string (e.g. X) as the password using HTTP Basic Authentication.\n  sources:\n  - openapi/freshdesk-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/authentication/freshdesk-authentication.yml
summary_line: http · 1 scheme
tags: []
---
