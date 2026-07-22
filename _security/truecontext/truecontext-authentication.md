---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Truecontext Authentication
name_suffix: Authentication
oauth_flows: []
overview: TrueContext secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TrueContext
provider_slug: truecontext
scheme_count: 1
schemes:
- description: API credential (key/secret pair) issued in the TrueContext portal and sent on each request to the versioned REST API. Exact header/parameter naming is documented in the authenticated product documentation at docs.truecontext.com.
  in: header
  name: apiKey
  sources:
  - docs.truecontext.com
  type: apiKey
slug: truecontext-authentication
source_filename: truecontext-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://docs.truecontext.com/ (TrueContext REST API documentation);\n  https://truecontext.com/product/integrations/?tab=api-integrations; live probe\n  of https://api.prontoforms.com/api/2.0/ (returns HTTP 401 without credentials).\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  notes: >-\n    The TrueContext (ProntoForms) REST API requires authenticated API credentials;\n    unauthenticated requests to api.prontoforms.com/api/1.0/ and /api/2.0/ return\n    HTTP 401. API access is an Elite-tier capability. Credentials are provisioned\n    and managed by an account administrator in the TrueContext web portal\n    (live.truecontext.com) rather than via a public self-serve OAuth app registry.\n    No OAuth2 authorization-server or OpenID configuration is published at the\n    provider's well-known endpoints (probed 404 / redirect-to-login).\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n    description:\
  \ >-\n      API credential (key/secret pair) issued in the TrueContext portal and sent\n      on each request to the versioned REST API. Exact header/parameter naming is\n      documented in the authenticated product documentation at docs.truecontext.com.\n    sources: [docs.truecontext.com]\ndocs: https://docs.truecontext.com/\nobserved:\n  - {host: api.prontoforms.com, path: /api/2.0/, status: 401}\n  - {host: api.prontoforms.com, path: /api/1.0/, status: 401}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truecontext/refs/heads/main/authentication/truecontext-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Field Service
- Mobile Forms
- Workflow Automation
- Data Collection
- Field Intelligence
- Low-Code
- Dispatch
- Inspections
- Compliance
---
