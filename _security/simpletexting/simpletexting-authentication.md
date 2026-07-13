---
api_key_in: []
api_specs:
- filename: simpletexting-openapi.yml
  format: yaml
  label: SimpleTexting Messages API
  slug: messages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-openapi.yml
- filename: simpletexting-openapi.yml
  format: yaml
  label: SimpleTexting Contacts API
  slug: contacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-openapi.yml
- filename: simpletexting-openapi.yml
  format: yaml
  label: SimpleTexting Lists API
  slug: lists
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-openapi.yml
- filename: simpletexting-openapi.yml
  format: yaml
  label: SimpleTexting Campaigns API
  slug: campaigns
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-openapi.yml
- filename: simpletexting-openapi.yml
  format: yaml
  label: SimpleTexting Autoresponders API
  slug: autoresponders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-openapi.yml
- filename: simpletexting-openapi.yml
  format: yaml
  label: SimpleTexting Sending Numbers API
  slug: sending-numbers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-openapi.yml
- filename: simpletexting-openapi.yml
  format: yaml
  label: SimpleTexting Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Simpletexting Authentication
name_suffix: Authentication
oauth_flows: []
overview: SimpleTexting secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SimpleTexting
provider_slug: simpletexting
scheme_count: 1
schemes:
- description: 'Send the API token as a bearer token in the Authorization header: `Authorization: Bearer <token>`. Generate a token in the SimpleTexting web app under Settings.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/simpletexting-openapi.yml
  type: http
slug: simpletexting-authentication
source_filename: simpletexting-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/simpletexting-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Send the API token as a bearer token in the Authorization header: `Authorization:\n    Bearer <token>`. Generate a token in the SimpleTexting web app under Settings.'\n  sources:\n  - openapi/simpletexting-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/authentication/simpletexting-authentication.yml
summary_line: http · 1 scheme
tags:
- SMS
- MMS
- Messaging
- Marketing
- Text Messaging
---
