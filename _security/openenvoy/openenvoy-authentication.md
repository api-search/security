---
api_key_in:
- header
api_specs:
- filename: openenvoy-job-api-openapi.yml
  format: yaml
  label: OpenEnvoy Job API
  slug: openenvoy-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openenvoy/refs/heads/main/openapi/openenvoy-job-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Openenvoy Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenEnvoy secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OpenEnvoy
provider_slug: openenvoy
scheme_count: 2
schemes:
- declared_in_spec: true
  format: Bearer {auth_token}
  in: header
  name: jwt
  parameter: Authorization
  required: true
  sources:
  - openapi/openenvoy-openapi.json
  - postman/openenvoy-postman-collection.json
  type: apiKey
- declared_in_spec: false
  in: header
  name: client-id
  note: Required on all 17 published operations but modelled as a plain header parameter rather than a securityDefinition. Present on every request in the Postman collection.
  parameter: X-CLIENT-ID
  required: true
  sources:
  - openapi/openenvoy-openapi.json
  - postman/openenvoy-postman-collection.json
  type: apiKey
slug: openenvoy-authentication
source_filename: openenvoy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://apidocs.openenvoy.io/ (collection description) + openapi/openenvoy-openapi.json\ndocs: https://apidocs.openenvoy.io/\nsummary:\n  model: dual-header static credential\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  note: >-\n    OpenEnvoy requires TWO headers on every request, not one. The published Swagger 2.0 definition\n    declares only the Authorization scheme as a securityDefinition and carries X-CLIENT-ID as an\n    ordinary required header parameter on each operation, so a generated client that honours only\n    securityDefinitions will send an incomplete credential and receive HTTP 400.\nschemes:\n- name: jwt\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Bearer {auth_token}'\n  required: true\n  declared_in_spec: true\n  sources:\n  - openapi/openenvoy-openapi.json\n  - postman/openenvoy-postman-collection.json\n- name:\
  \ client-id\n  type: apiKey\n  in: header\n  parameter: X-CLIENT-ID\n  required: true\n  declared_in_spec: false\n  note: >-\n    Required on all 17 published operations but modelled as a plain header parameter rather than a\n    securityDefinition. Present on every request in the Postman collection.\n  sources:\n  - openapi/openenvoy-openapi.json\n  - postman/openenvoy-postman-collection.json\ncredential_issuance:\n  self_serve: false\n  method: contact-customer-success\n  contact: support@openenvoy.com\n  statement: >-\n    \"If you are an existing customer, please contact our customer success team at\n    support@openenvoy.com for client_id and auth_token. Keep them in a secure place.\"\n  source: https://apidocs.openenvoy.io/\n  note: >-\n    Credentials are issued to existing customers only; there is no public self-service key\n    provisioning on the developer surface. OpenEnvoy's own newsroom describes a self-serve API in\n    which a user generates an API key from inside the product,\
  \ which is an authenticated\n    in-product flow rather than an anonymous developer signup.\nrotation:\n  documented: false\n  note: No credential rotation, expiry or revocation policy is published on the public docs surface.\nobserved:\n  - probe: 'GET https://backend.openenvoy.io/public/api/v1/jobs/1 (no headers)'\n    http_status: 400\n    body: '{\"errorCode\":\"E00400\",\"errorMessage\":\"Invalid/Missing Header\",\"key\":\"Authorization\"}'\n    note: >-\n      Anonymous probe on 2026-08-26. The API rejects a missing credential with HTTP 400 and a\n      structured error naming the offending header, not the conventional 401 Unauthorized.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openenvoy/refs/heads/main/authentication/openenvoy-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Accounts Payable
- Accounts Receivable
- Invoice Processing
- Finance Automation
- Accounting
- Procure-to-Pay
- Document Processing
- Artificial Intelligence
- ERP Integration
- Spend Management
---
