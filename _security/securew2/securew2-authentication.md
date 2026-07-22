---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Securew2 Authentication
name_suffix: Authentication
oauth_flows: []
overview: SecureW2 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SecureW2
provider_slug: securew2
scheme_count: 1
schemes:
- access_levels:
  - Read-Only
  - Read-Write
  format: Bearer <API Secret>
  header: Authorization
  location: header
  name: bearerAuth
  scheme: bearer
  sources:
  - docs:rest-api-based-organization-provisioning-for-msps
  token_source: JoinNow Management Portal (REST API Organization Management Token)
  type: http
slug: securew2-authentication
source_filename: securew2-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://securew2.com/documentation/rest-api-based-organization-provisioning-for-msps\ndocs: https://securew2.com/documentation/rest-api-based-organization-provisioning-for-msps\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  oauth2_flows: []\n  notes: >-\n    The SecureW2 REST API for MSP organization provisioning authenticates with a\n    bearer token. A \"REST API Organization Management Token\" is generated in the\n    JoinNow Management Portal and downloaded as a CSV containing an API Key ID and\n    API Secret. The secret is presented on each request in the Authorization header\n    as \"Bearer <secret>\". Tokens can be scoped Read-Only (GET) or Read-Write\n    (GET/POST/PATCH) and require an APEX, Guardian, or Campus license.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  location: header\n  header: Authorization\n  format: 'Bearer <API Secret>'\n  token_source: JoinNow Management Portal\
  \ (REST API Organization Management Token)\n  access_levels:\n  - Read-Only\n  - Read-Write\n  sources:\n  - docs:rest-api-based-organization-provisioning-for-msps\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/securew2/refs/heads/main/authentication/securew2-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cybersecurity
- Authentication
- PKI
- Certificates
- Network Security
- Passwordless
- RADIUS
- Identity
- MSP
---
