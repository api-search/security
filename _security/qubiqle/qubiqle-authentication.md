---
api_key_in:
- header
api_specs:
- filename: qubiqle-openapi-original.json
  format: json
  label: Ottimate API V1
  slug: ottimate-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubiqle/refs/heads/main/openapi/qubiqle-openapi-original.json
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Qubiqle Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Qubiqle secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Qubiqle
provider_slug: qubiqle
scheme_count: 2
schemes:
- description: Bearer access token from the OAuth2 client_credentials grant. Obtained by POSTing client_id + client_secret to the environment auth server (sandbox-auth.ottimate.com / auth.ottimate.com). Tokens are cached until expires_in elapses or a 401 is returned.
  name: OAuth2
  scheme: bearer
  sources:
  - openapi/qubiqle-openapi-original.json
  token_urls:
    production: https://auth.ottimate.com/oauth/token
    sandbox: https://sandbox-auth.ottimate.com/oauth/token
  type: http
- description: Partner-provisioned API key, required on every request in addition to the bearer token. Rotating the key invalidates cached idempotency entries scoped to it.
  in: header
  name: X-Api-Key
  parameter: X-Api-Key
  sources:
  - openapi/qubiqle-openapi-original.json
  - https://docs.ottimate.com/auth
  type: apiKey
slug: qubiqle-authentication
source_filename: qubiqle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/qubiqle-openapi-original.json\ndocs: https://docs.ottimate.com/auth\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  notes: >-\n    Every request requires BOTH an X-Api-Key header (partner-provisioned API key)\n    and an Authorization: Bearer access token obtained via the OAuth2\n    client_credentials grant. Client ID / Client Secret and API keys are\n    provisioned per client account by an Ottimate Partner Manager (no\n    self-service). Only the scope accounts.can_access_dashboard is currently\n    supported. Auth server URLs differ by environment.\nschemes:\n- name: OAuth2\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer access token from the OAuth2 client_credentials grant. Obtained by\n    POSTing client_id + client_secret to the environment auth server\n    (sandbox-auth.ottimate.com / auth.ottimate.com). Tokens are cached until\n\
  \    expires_in elapses or a 401 is returned.\n  token_urls:\n    sandbox: https://sandbox-auth.ottimate.com/oauth/token\n    production: https://auth.ottimate.com/oauth/token\n  sources:\n  - openapi/qubiqle-openapi-original.json\n- name: X-Api-Key\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: >-\n    Partner-provisioned API key, required on every request in addition to the\n    bearer token. Rotating the key invalidates cached idempotency entries scoped\n    to it.\n  sources:\n  - openapi/qubiqle-openapi-original.json\n  - https://docs.ottimate.com/auth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qubiqle/refs/heads/main/authentication/qubiqle-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Accounts Payable
- Invoicing
- Payments
- Accounting
- FinTech
- Automation
- Artificial Intelligence
- ERP Integration
- Procurement
---
