---
api_key_in:
- header
api_specs:
- filename: agave-budgets-api-openapi.yml
  format: yaml
  label: Agave Budgets API
  slug: agave-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-budgets-api-openapi.yml
- filename: agave-contracts-api-openapi.yml
  format: yaml
  label: Agave Contracts API
  slug: agave-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-contracts-api-openapi.yml
- filename: agave-cost-codes-api-openapi.yml
  format: yaml
  label: Agave Cost Codes API
  slug: agave-cost-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-cost-codes-api-openapi.yml
- filename: agave-employees-api-openapi.yml
  format: yaml
  label: Agave Employees API
  slug: agave-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-employees-api-openapi.yml
- filename: agave-invoices-api-openapi.yml
  format: yaml
  label: Agave Invoices API
  slug: agave-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-invoices-api-openapi.yml
- filename: agave-link-sessions-api-openapi.yml
  format: yaml
  label: Agave Link Sessions API
  slug: agave-link-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-link-sessions-api-openapi.yml
- filename: agave-projects-api-openapi.yml
  format: yaml
  label: Agave Projects API
  slug: agave-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-projects-api-openapi.yml
- filename: agave-timesheets-api-openapi.yml
  format: yaml
  label: Agave Timesheets API
  slug: agave-timesheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-timesheets-api-openapi.yml
- filename: agave-vendors-api-openapi.yml
  format: yaml
  label: Agave Vendors API
  slug: agave-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-vendors-api-openapi.yml
auth_types:
- apiKey
description: 'Agave''s own API authenticates with three static credential headers plus a required version header; there is no OAuth, no bearer token and no token endpoint on the Agave API itself. OAuth exists in the product, but one layer down: Agave Link runs the OAuth dance against each SOURCE SYSTEM (Procore, Autodesk, QuickBooks, ...) on the user''s behalf and hands back an opaque Account Token. So a caller holds long-lived, non-expiring, non-scoped credentials that grant whatever the linked user granted — there is nothing to narrow. This artifact replaces an earlier derived profile that recorded a single "API-Key" header scheme; that scheme was an artefact of an API Evangelist-authored spec and does not exist on the live API. Verified live 2026-08-30: GET https://api.agaveapi.com/projects returns 401 {"error":"Invalid API-Version header"}.'
kind: authentication
layout: security
method: searched
name: Agave Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agave secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Agave
provider_slug: agave
scheme_count: 3
schemes:
- description: Identifies the integrating application.
  format: 36-character UUID
  in: header
  issued_by: Agave (api-support@agaveapi.com)
  name: ClientId
  parameter: Client-Id
  required: true
  sources:
  - https://docs.agaveapi.com/agave-api/headers
  type: apiKey
- description: Secret paired with Client-Id. Must never reach a browser.
  format: 40-character string
  in: header
  issued_by: Agave (api-support@agaveapi.com)
  name: ClientSecret
  parameter: Client-Secret
  required: true
  sources:
  - https://docs.agaveapi.com/agave-api/headers
  type: apiKey
- description: Per-linked-account token returned after exchanging the Agave Link public token. Selects WHICH end-customer source-system account the request acts against.
  in: header
  name: AccountToken
  parameter: Account-Token
  required: true
  required_except: '"Link Token" requests, where it is not applicable'
  sources:
  - https://docs.agaveapi.com/agave-api/headers
  type: apiKey
slug: agave-authentication
source_filename: agave-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: https://docs.agaveapi.com/agave-api/headers\ndocs:\n- https://docs.agaveapi.com/agave-api/headers\n- https://docs.agaveapi.com/agave-api/identifiers\n- https://docs.agaveapi.com/agave-link/authentication-flow\n- https://docs.agaveapi.com/agave-api/api-versioning\ndescription: >-\n  Agave's own API authenticates with three static credential headers plus a required version header;\n  there is no OAuth, no bearer token and no token endpoint on the Agave API itself. OAuth exists in\n  the product, but one layer down: Agave Link runs the OAuth dance against each SOURCE SYSTEM\n  (Procore, Autodesk, QuickBooks, ...) on the user's behalf and hands back an opaque Account Token.\n  So a caller holds long-lived, non-expiring, non-scoped credentials that grant whatever the linked\n  user granted — there is nothing to narrow. This artifact replaces an earlier derived profile that\n  recorded a single \"API-Key\" header scheme; that scheme\
  \ was an artefact of an API Evangelist-authored\n  spec and does not exist on the live API. Verified live 2026-08-30: GET\n  https://api.agaveapi.com/projects returns 401 {\"error\":\"Invalid API-Version header\"}.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  credential_count: 3\n  version_header_required: true\n  scopes: none\n  token_expiry: none documented\n  rotation: not documented\nschemes:\n- name: ClientId\n  type: apiKey\n  in: header\n  parameter: Client-Id\n  required: true\n  format: 36-character UUID\n  issued_by: Agave (api-support@agaveapi.com)\n  description: Identifies the integrating application.\n  sources: [https://docs.agaveapi.com/agave-api/headers]\n- name: ClientSecret\n  type: apiKey\n  in: header\n  parameter: Client-Secret\n  required: true\n  format: 40-character string\n  issued_by: Agave (api-support@agaveapi.com)\n  description: Secret paired with Client-Id. Must never reach a browser.\n  sources: [https://docs.agaveapi.com/agave-api/headers]\n\
  - name: AccountToken\n  type: apiKey\n  in: header\n  parameter: Account-Token\n  required: true\n  required_except: '\"Link Token\" requests, where it is not applicable'\n  description: >-\n    Per-linked-account token returned after exchanging the Agave Link public token. Selects WHICH\n    end-customer source-system account the request acts against.\n  sources: [https://docs.agaveapi.com/agave-api/headers]\nversion_gate:\n  parameter: API-Version\n  required: true\n  current: '2021-11-21'\n  failure: 401 with {\"message\":\"Invalid API-Version header\"}\n  note: Enforced before authentication — a request without it fails 401 even with valid credentials.\nscoping_headers:\n- name: Project-Id\n  description: Agave Project UUID, scoping the request to one project in PM/field-service systems. Accepts \"*\" on some endpoints.\n- name: Company-Id\n  description: Agave Company UUID, used when the user granted cross-company access. Enumerate via /link/companies.\ndelegated_auth:\n  mechanism:\
  \ Agave Link\n  flow: >-\n    Create a Link Token (POST /link/token with a reference_id) -> open the hosted Agave Link component\n    -> the user authenticates with their source system -> onSuccess returns a publicToken -> exchange\n    it (POST /link/token/exchange) for a long-lived Account-Token.\n  docs: https://docs.agaveapi.com/agave-link/authentication-flow\n  reference_id:\n    description: >-\n      Opaque caller-chosen string, max 255 characters, that identifies the integration/user pair. One\n      reference_id belongs to exactly one integration; on-prem and hosted source systems (QuickBooks\n      Desktop, Foundation, Vista, Sage 100/300, ComputerEase, Cheops) require the SAME reference_id to\n      re-authenticate the same user, and a different one yields different Agave ids for the same\n      underlying object.\n    docs: https://docs.agaveapi.com/agave-api/reference-id\n  single_sign_on: https://docs.agaveapi.com/agave-link/single-sign-on\ngaps:\n- No OAuth 2.0 or OpenID\
  \ Connect on Agave's own API — no authorization or token endpoint, no scopes.\n- No documented credential expiry, rotation procedure, or revocation endpoint for Client-Secret.\n- >-\n  Account tokens can be revoked administratively (POST /admin/accounts/{id}/revoke-tokens appears in\n  Agave's Postman collection) but that operation is not covered in the published docs.\n- Credentials are obtained by emailing api-support@agaveapi.com, not through self-serve issuance.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/authentication/agave-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Accounting
- Construction
- Integration
- ERP
- Project Management
- Unified-API
- iPaaS
- Webhook
- Field Service
- Invoicing
---
