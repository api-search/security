---
api_key_in: []
api_specs:
- filename: ascend-advanced-therapies-wp-rest-openapi.yml
  format: yaml
  label: Ascend Advanced Therapies Content API (WordPress REST)
  slug: wp-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ascend-advanced-therapies/refs/heads/main/openapi/ascend-advanced-therapies-wp-rest-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Ascend Advanced Therapies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ascend Advanced Therapies secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ascend Advanced Therapies
provider_slug: ascend-advanced-therapies
scheme_count: 1
schemes:
- advertised_at: https://www.ascend-adv.com/wp-json/
  authorization_url: https://www.ascend-adv.com/wp-admin/authorize-application.php
  description: WordPress Application Passwords. Credentials are a WordPress username plus a generated application password, presented as HTTP Basic over TLS. Required only for write operations and for privileged reads; the entire public content surface is readable without credentials.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/ascend-advanced-therapies-wp-rest-openapi.yml
  - https://www.ascend-adv.com/wp-json/
  type: http
slug: ascend-advanced-therapies-authentication
source_filename: ascend-advanced-therapies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.ascend-adv.com/wp-json/\ndocs: https://www.ascend-adv.com/wp-admin/authorize-application.php\nnote: >-\n  Upgraded from derived to searched: the live WordPress REST discovery document at\n  https://www.ascend-adv.com/wp-json/ advertises the supported authentication method directly in its\n  `authentication` block. Anonymous access was verified against every read operation captured in\n  openapi/ascend-advanced-therapies-wp-rest-openapi.yml (all returned HTTP 200); privileged routes\n  such as /wp/v2/settings and /wp/v2/block-types returned HTTP 401 anonymously.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  anonymous_read: true\n  oauth2_flows: []\n  api_key_in: []\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: >-\n    WordPress Application Passwords. Credentials are a WordPress username plus a generated\n    application password, presented as HTTP Basic over\
  \ TLS. Required only for write operations and\n    for privileged reads; the entire public content surface is readable without credentials.\n  authorization_url: https://www.ascend-adv.com/wp-admin/authorize-application.php\n  advertised_at: https://www.ascend-adv.com/wp-json/\n  sources:\n  - openapi/ascend-advanced-therapies-wp-rest-openapi.yml\n  - https://www.ascend-adv.com/wp-json/\nevidence:\n- source: https://www.ascend-adv.com/wp-json/\n  field: authentication.application-passwords.endpoints.authorization\n  value: https://www.ascend-adv.com/wp-admin/authorize-application.php\n- probe: GET /wp/v2/posts?per_page=1\n  status: 200\n  anonymous: true\n- probe: GET /wp/v2/settings\n  status: 401\n  anonymous: true\n  body_code: rest_forbidden\n- probe: GET /wp/v2/block-types\n  status: 401\n  anonymous: true\nunsupported:\n- oauth2\n- openIdConnect\n- mutualTLS\n- apiKey\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ascend-advanced-therapies/refs/heads/main/authentication/ascend-advanced-therapies-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Biotechnology
- Gene Therapy
- Cell Therapy
- Contract Manufacturing
- Life Sciences
- Pharmaceuticals
- CDMO
- AAV
---
