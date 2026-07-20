---
api_key_in: []
api_specs:
- filename: arpeggi-labs-kits-openapi.yml
  format: yaml
  label: Kits AI API
  slug: kits-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arpeggi-labs/refs/heads/main/openapi/arpeggi-labs-kits-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Arpeggi Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arpeggi Labs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Arpeggi Labs
provider_slug: arpeggi-labs
scheme_count: 1
schemes:
- description: 'API key issued from the Kits AI API access page (https://app.kits.ai/api-access), sent as `Authorization: Bearer <api-key>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/arpeggi-labs-kits-openapi.yml
  type: http
slug: arpeggi-labs-authentication
source_filename: arpeggi-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/arpeggi-labs-kits-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key issued from the Kits AI API access page (https://app.kits.ai/api-access),\n    sent as `Authorization: Bearer <api-key>`.'\n  sources:\n  - openapi/arpeggi-labs-kits-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arpeggi-labs/refs/heads/main/authentication/arpeggi-labs-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Music
- Audio
- Artificial Intelligence
- Voice
- Machine Learning
- Generative AI
- Media
---
