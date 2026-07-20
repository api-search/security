---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Column Tax Authentication
name_suffix: Authentication
oauth_flows: []
overview: Column Tax secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Column Tax
provider_slug: column-tax
scheme_count: 1
schemes:
- description: HTTP Basic authentication. The Authorization header carries Base64-encoded client_id:client_secret. Every request must include this header.
  format: Basic base64(client_id:client_secret)
  header: Authorization
  location: header
  name: basicAuth
  scheme: basic
  sources:
  - https://docs.columntax.com/reference/authentication
  type: http
slug: column-tax-authentication
source_filename: column-tax-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.columntax.com/reference/authentication\ndocs: https://docs.columntax.com/reference/authentication\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  credential_provisioning: manual\n  notes: 'Credentials (client_id and client_secret) are provisioned by the Column Tax team and must be\n    stored in secure credentials storage. All API calls are made server-side to keep the client_secret\n    off the client.'\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'HTTP Basic authentication. The Authorization header carries Base64-encoded\n    client_id:client_secret. Every request must include this header.'\n  location: header\n  header: Authorization\n  format: 'Basic base64(client_id:client_secret)'\n  sources: [https://docs.columntax.com/reference/authentication]\nrequired_headers:\n- name: Authorization\n  value: 'Basic <base64(client_id:client_secret)>'\n  applies_to: all requests\n\
  - name: Content-Type\n  value: application/json\n  applies_to: POST requests\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/column-tax/refs/heads/main/authentication/column-tax-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Tax
- Tax Filing
- Embedded Finance
- E-File
- Financial Services
- Banking
- API First
---
