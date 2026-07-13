---
api_key_in:
- query
api_specs:
- filename: olark-openapi.yml
  format: yaml
  label: Olark JavaScript API
  slug: javascript-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/olark/refs/heads/main/openapi/olark-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Olark Authentication
name_suffix: Authentication
oauth_flows: []
overview: Olark secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Olark
provider_slug: olark
scheme_count: 1
schemes:
- description: 'Olark identifies an installation via a public site identifier

    (e.g. `1234-456-78-9810`) passed client-side to `olark.identify()`.

    It is not a secret and is included here only to make the

    identification mechanism explicit in the OpenAPI contract.'
  in: query
  name: OlarkSiteId
  parameter: site_id
  sources:
  - openapi/olark-openapi.yml
  type: apiKey
slug: olark-authentication
source_filename: olark-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/olark-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: OlarkSiteId\n  type: apiKey\n  in: query\n  parameter: site_id\n  description: |-\n    Olark identifies an installation via a public site identifier\n    (e.g. `1234-456-78-9810`) passed client-side to `olark.identify()`.\n    It is not a secret and is included here only to make the\n    identification mechanism explicit in the OpenAPI contract.\n  sources:\n  - openapi/olark-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/olark/refs/heads/main/authentication/olark-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Live Chat
- Customer Support
- Chatbots
- Customer Engagement
- Messaging
- Accessibility
---
