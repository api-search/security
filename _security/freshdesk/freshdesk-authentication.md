---
api_key_in: []
api_specs:
- filename: freshdesk-rest-api-openapi.yml
  format: yaml
  label: Freshdesk REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-rest-api-openapi.yml
- filename: freshdesk-webhook-api-asyncapi.yml
  format: yaml
  label: Freshdesk Webhook API
  slug: webhook-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/asyncapi/freshdesk-webhook-api-asyncapi.yml
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
