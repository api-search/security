---
api_key_in: []
api_specs:
- filename: crisp-openapi.yml
  format: yaml
  label: Crisp REST API v1
  slug: crisp-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crisp/refs/heads/main/openapi/crisp-openapi.yml
- filename: crisp-asyncapi.yml
  format: yaml
  label: Crisp Realtime (Webhooks + RTM) v1
  slug: crisp-realtime-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/crisp/refs/heads/main/asyncapi/crisp-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Crisp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crisp secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Crisp
provider_slug: crisp
scheme_count: 1
schemes:
- description: 'Use plugin token credentials. HTTP Basic with identifier:key, plus

    the X-Crisp-Tier header (`plugin`, `user`, or `tier`).'
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/crisp-openapi.yml
  type: http
slug: crisp-authentication
source_filename: crisp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/crisp-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: |-\n    Use plugin token credentials. HTTP Basic with identifier:key, plus\n    the X-Crisp-Tier header (`plugin`, `user`, or `tier`).\n  sources:\n  - openapi/crisp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crisp/refs/heads/main/authentication/crisp-authentication.yml
summary_line: http · 1 scheme
tags:
- Customer Service
- Live Chat
- Helpdesk
- Messaging
- Chatbots
---
