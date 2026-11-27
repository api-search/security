---
anonymous_access: false
api_key_in: []
api_specs:
- filename: docmorph-dev-tools-api-openapi.yml
  format: yaml
  label: DocMorph Tools API
  slug: docmorph-dev-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docmorph-dev/openapi/docmorph-dev-tools-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: DocMorph Authentication
name_suffix: Authentication
oauth_flows: []
overview: DocMorph secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DocMorph
provider_slug: docmorph-dev
scheme_count: 1
schemes:
- bearerFormat: JWT/HMAC
  description: Optional VIP or Developer API Token. Free tier requests are accepted without a token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/docmorph-dev-openapi.json
  type: http
slug: docmorph-dev-authentication
source_filename: docmorph-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/docmorph-dev-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT/HMAC\n  description: Optional VIP or Developer API Token. Free tier requests are accepted without\n    a token.\n  sources:\n  - openapi/docmorph-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/docmorph-dev/authentication/docmorph-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Document Processing
- Privacy
- OCR
- Media
- Local-First
---
