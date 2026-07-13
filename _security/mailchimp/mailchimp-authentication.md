---
api_key_in:
- header
api_specs:
- filename: mailchimp-marketing-api-openapi.yml
  format: yaml
  label: Mailchimp Marketing API
  slug: mailchimp-marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/openapi/mailchimp-marketing-api-openapi.yml
- filename: mailchimp-transactional-api-openapi.yml
  format: yaml
  label: Mailchimp Transactional API
  slug: mailchimp-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/openapi/mailchimp-transactional-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mailchimp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mailchimp secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mailchimp
provider_slug: mailchimp
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/mailchimp-marketing-api-openapi.yml
  type: http
- description: Mandrill uses API key authentication. The key is passed in the JSON request body as the "key" parameter for every call, or alternatively via the X-MC-ApiKey header.
  in: header
  name: apiKey
  parameter: X-MC-ApiKey
  sources:
  - openapi/mailchimp-transactional-api-openapi.yml
  type: apiKey
slug: mailchimp-authentication
source_filename: mailchimp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mailchimp-marketing-api-openapi.yml, openapi/mailchimp-transactional-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/mailchimp-marketing-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-MC-ApiKey\n  description: Mandrill uses API key authentication. The key is passed in the JSON request body\n    as the \"key\" parameter for every call, or alternatively via the X-MC-ApiKey header.\n  sources:\n  - openapi/mailchimp-transactional-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/authentication/mailchimp-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
---
