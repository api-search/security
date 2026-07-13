---
api_key_in: []
api_specs:
- filename: missive-rest-api-openapi.yml
  format: yaml
  label: Missive REST API
  slug: missive-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/missive/refs/heads/main/openapi/missive-rest-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Missive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Missive secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Missive
provider_slug: missive
scheme_count: 1
schemes:
- description: 'Personal access token generated in Missive preferences. Format: Bearer missive_pat-[token]. Requires Productive plan or higher.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/missive-rest-api-openapi.yml
  type: http
slug: missive-authentication
source_filename: missive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/missive-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Personal access token generated in Missive preferences. Format: Bearer missive_pat-[token].\n    Requires Productive plan or higher.'\n  sources:\n  - openapi/missive-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/missive/refs/heads/main/authentication/missive-authentication.yml
summary_line: http · 1 scheme
tags:
- Team Inbox
- Collaboration
- Email
- Messaging
- Conversations
- Contacts
- Webhooks
- Automation
- REST API
---
