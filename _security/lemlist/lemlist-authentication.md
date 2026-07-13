---
api_key_in: []
api_specs:
- filename: lemlist-openapi.yml
  format: yaml
  label: lemlist REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lemlist Authentication
name_suffix: Authentication
oauth_flows: []
overview: lemlist secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: lemlist
provider_slug: lemlist
scheme_count: 1
schemes:
- description: 'HTTP Basic Authentication. The login is always empty and the

    password is your lemlist API key. Send the header as

    `Authorization: Basic ` followed by the base64 encoding of

    `:YOUR_API_KEY`.'
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/lemlist-openapi.yml
  type: http
slug: lemlist-authentication
source_filename: lemlist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lemlist-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic Authentication. The login is always empty and the\n    password is your lemlist API key. Send the header as\n    `Authorization: Basic ` followed by the base64 encoding of\n    `:YOUR_API_KEY`.\n  sources:\n  - openapi/lemlist-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/authentication/lemlist-authentication.yml
summary_line: http · 1 scheme
tags:
- Email Outreach
- Sales Engagement
- Cold Email
- Sales Automation
- LinkedIn Outreach
- Lead Generation
---
