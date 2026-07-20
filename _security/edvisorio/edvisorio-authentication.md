---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Edvisorio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Edvisor.io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Edvisor.io
provider_slug: edvisorio
scheme_count: 1
schemes:
- description: Edvisor.io uses long-lived API keys presented as an HTTP Bearer token in the Authorization header on every request to the GraphQL API (https://api-v2.edvisor.io/graphql).
  format: 'Authorization: Bearer <your_edvisor_api_key>'
  header: Authorization
  in: header
  name: bearerApiKey
  notes: Edvisor requires all requests be made from a server, never a customer-facing front end, to avoid exposing the key. School Company API keys can be retrieved via the getSchoolCompanyApiKey GraphQL query.
  provisioning: API keys are issued on request by Edvisor support (contact support@edvisor.io); there is no self-service key management surface documented.
  scheme: bearer
  server_side_only: true
  type: http
slug: edvisorio-authentication
source_filename: edvisorio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.edvisor.io/\ndocs: https://docs.edvisor.io/\nsummary:\n  types: [http]\n  http_scheme: bearer\n  token_type: api-key\n  oauth2_flows: []\n  api_key_in: [header]\nschemes:\n  - name: bearerApiKey\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: \"Authorization: Bearer <your_edvisor_api_key>\"\n    description: >-\n      Edvisor.io uses long-lived API keys presented as an HTTP Bearer token in the\n      Authorization header on every request to the GraphQL API\n      (https://api-v2.edvisor.io/graphql).\n    provisioning: >-\n      API keys are issued on request by Edvisor support (contact support@edvisor.io);\n      there is no self-service key management surface documented.\n    server_side_only: true\n    notes: >-\n      Edvisor requires all requests be made from a server, never a customer-facing\n      front end, to avoid exposing the key. School Company API keys can\
  \ be retrieved\n      via the getSchoolCompanyApiKey GraphQL query.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edvisorio/refs/heads/main/authentication/edvisorio-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Education
- Student Recruitment
- International Education
- EdTech
- GraphQL
- Marketplace
- Webhooks
---
