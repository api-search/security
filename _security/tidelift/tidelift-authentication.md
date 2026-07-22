---
api_key_in: []
api_specs:
- filename: tidelift-subscriber-api-openapi-original.json
  format: json
  label: Tidelift External API
  slug: tidelift-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidelift/refs/heads/main/openapi/tidelift-subscriber-api-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Tidelift Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tidelift secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tidelift
provider_slug: tidelift
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/tidelift-subscriber-api-openapi-original.json
  type: http
slug: tidelift-authentication
source_filename: tidelift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/tidelift-subscriber-api-openapi-original.json\ndocs: https://docs.tidelift.com/article/79-api-authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  key_types:\n  - user\n  - project\n  - organization\n  note: >-\n    A Tidelift API key is required for all External API endpoints, passed as a Bearer token\n    in the Authorization header. The security requirement declares three key scopes\n    (user, project, organization); each path documents which key type it accepts.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/tidelift-subscriber-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tidelift/refs/heads/main/authentication/tidelift-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Open Source
- Software Supply Chain
- Dependency Management
- Application Security
- SBOM
- License Compliance
- Vulnerability Management
- Developer Tools
---
