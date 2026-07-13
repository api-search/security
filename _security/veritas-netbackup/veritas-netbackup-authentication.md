---
api_key_in: []
api_specs:
- filename: veritas-netbackup-rest-api-openapi.yml
  format: yaml
  label: Veritas NetBackup REST API
  slug: veritas-netbackup-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veritas-netbackup/refs/heads/main/openapi/veritas-netbackup-rest-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Veritas Netbackup Authentication
name_suffix: Authentication
oauth_flows: []
overview: Veritas NetBackup secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Veritas NetBackup
provider_slug: veritas-netbackup
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'JSON Web Token obtained from the /login endpoint. Include in the Authorization header as: Bearer <token>'
  name: jwtAuth
  scheme: bearer
  sources:
  - openapi/veritas-netbackup-rest-api-openapi.yml
  type: http
slug: veritas-netbackup-authentication
source_filename: veritas-netbackup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/veritas-netbackup-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: jwtAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'JSON Web Token obtained from the /login endpoint. Include in the Authorization\n    header as: Bearer <token>'\n  sources:\n  - openapi/veritas-netbackup-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veritas-netbackup/refs/heads/main/authentication/veritas-netbackup-authentication.yml
summary_line: http · 1 scheme
tags:
- Backup
- Data Protection
- Disaster Recovery
- Enterprise
- Recovery
- Storage
---
