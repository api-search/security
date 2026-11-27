---
anonymous_access: false
api_key_in:
- header
- query
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Tidy Byte Tools Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tidy Byte Tools secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tidy Byte Tools
provider_slug: tidybytetools
scheme_count: 3
schemes:
- description: 'A free key from POST /keys, as: Bearer tbt_...'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tidybytetools-openapi.json
  type: http
- in: header
  name: apiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/tidybytetools-openapi.json
  type: apiKey
- description: Allowed. Never put a key in the URL path.
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/tidybytetools-openapi.json
  type: apiKey
slug: tidybytetools-authentication
source_filename: tidybytetools-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/tidybytetools-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'A free key from POST /keys, as: Bearer tbt_...'\n  sources:\n  - openapi/tidybytetools-openapi.json\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/tidybytetools-openapi.json\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Allowed. Never put a key in the URL path.\n  sources:\n  - openapi/tidybytetools-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/tidybytetools/authentication/tidybytetools-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Data Transformation
- Utilities
- Free
- Edge Computing
---
