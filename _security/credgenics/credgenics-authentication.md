---
api_key_in:
- header
api_specs:
- filename: credgenics-recovery-openapi.yml
  format: yaml
  label: Credgenics Recovery API
  slug: credgenics-recovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credgenics/refs/heads/main/openapi/credgenics-recovery-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Credgenics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Credgenics secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Credgenics
provider_slug: credgenics
scheme_count: 1
schemes:
- description: Short-lived API token supplied in the `authenticationtoken` header on every resource request. Obtained by exchanging client credentials at POST /user/public/access-token.
  in: header
  name: authenticationToken
  parameter: authenticationtoken
  sources:
  - openapi/credgenics-recovery-openapi.yml
  type: apiKey
slug: credgenics-authentication
source_filename: credgenics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/credgenics-recovery-openapi.yml\ndocs: https://docs.credgenics.com/#getting-started\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  model: client-credentials-exchange\nschemes:\n- name: authenticationToken\n  type: apiKey\n  in: header\n  parameter: authenticationtoken\n  description: >-\n    Short-lived API token supplied in the `authenticationtoken` header on every\n    resource request. Obtained by exchanging client credentials at\n    POST /user/public/access-token.\n  sources:\n  - openapi/credgenics-recovery-openapi.yml\nflow:\n  token_endpoint: https://apiprod.credgenics.com/user/public/access-token\n  grant: client_credentials\n  request_fields: [client_id, client_secret, token_expiry_duration]\n  response_token_field: api_key\n  header: authenticationtoken\n  tenant_scoping:\n    parameter: company_id\n    location: query\n    required: true\n  token_expiry_default_seconds: 900\n  token_expiry_max_seconds:\
  \ 86400\n  client_secret_validity: 6 months\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credgenics/refs/heads/main/authentication/credgenics-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Enterprise
- Financial Services
- Debt Collection
- Loan Recovery
- Lending
- Collections
- Fintech
- India
---
