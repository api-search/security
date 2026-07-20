---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Class Authentication
name_suffix: Authentication
oauth_flows: []
overview: Class secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Class
provider_slug: class
scheme_count: 1
schemes:
- description: 'Authorization: Bearer [api_key_secret]. The bearer credential is a Class API key secret generated in the admin portal; each key carries a scope set and optional expiration.'
  name: bearerApiKey
  scheme: bearer
  sources:
  - https://developer.class.com
  type: http
slug: class-authentication
source_filename: class-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.class.com\ndocs: https://developer.class.com\nsummary:\n  types: [http]\n  http_scheme: bearer\n  key_style: api-key\n  scoped: true\n  notes: >-\n    API keys are minted in the Class admin portal (API Keys section) with a\n    selectable scope set and an optional expiration date. The one-time secret is\n    shown once on creation. Requests authenticate with an HTTP Bearer token.\nschemes:\n  - name: bearerApiKey\n    type: http\n    scheme: bearer\n    description: >-\n      Authorization: Bearer [api_key_secret]. The bearer credential is a Class\n      API key secret generated in the admin portal; each key carries a scope set\n      and optional expiration.\n    sources: [https://developer.class.com]\nscopes:\n  note: >-\n    Scopes are attached to each API key (not an OAuth2 flow). Selecting a write\n    scope automatically grants the matching read scope. Each endpoint documents\n    its required scope.\n\
  \  values:\n    - class:read\n    - class:write\n    - enrollment:read\n    - enrollment:write\n    - attendance:read\n    - metrics:read\n    - schedule:read\n    - schedule:write\n    - template:read\n    - template:write\n    - user:read\n    - user:write\nbase_url: >-\n  Class assigns each organization a unique base URL, found on the API Keys page.\n  Endpoints follow [api_base_url]/api/v1/[resource].\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/class/refs/heads/main/authentication/class-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Edtech
- Education
- Virtual Classroom
- Learning
- LMS
- Video Conferencing
- Live Learning
---
