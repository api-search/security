---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kontent Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kontent AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kontent AI
provider_slug: kontent-ai
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Send `Authorization: Bearer <YOUR_DELIVERY_API_KEY>`. Required for

    secure delivery, preview delivery, and secured asset access. The

    default public Delivery API does not require authentication.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/kontent-ai-openapi.yml
  type: http
slug: kontent-ai-authentication
source_filename: kontent-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kontent-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Send `Authorization: Bearer <YOUR_DELIVERY_API_KEY>`. Required for\n    secure delivery, preview delivery, and secured asset access. The\n    default public Delivery API does not require authentication.\n  sources:\n  - openapi/kontent-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kontent-ai/refs/heads/main/authentication/kontent-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- CMS
- Content
- GraphQL
- Headless CMS
---
