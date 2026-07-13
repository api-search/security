---
api_key_in:
- header
api_specs:
- filename: bill-webhooks-asyncapi.yml
  format: yaml
  label: BILL v3 API
  slug: v3-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bill/refs/heads/main/asyncapi/bill-webhooks-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bill Authentication
name_suffix: Authentication
oauth_flows: []
overview: BILL secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BILL
provider_slug: bill
scheme_count: 1
schemes:
- description: 'Session identifier obtained from `POST /login`. Expires after 35 minutes

    of inactivity. A `devKey` (developer key) is also required on requests

    and is sent alongside `sessionId` in the appropriate header per BILL''s

    official reference.'
  in: header
  name: sessionAuth
  parameter: sessionId
  sources:
  - openapi/bill-openapi.yml
  type: apiKey
slug: bill-authentication
source_filename: bill-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bill-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sessionAuth\n  type: apiKey\n  in: header\n  parameter: sessionId\n  description: |-\n    Session identifier obtained from `POST /login`. Expires after 35 minutes\n    of inactivity. A `devKey` (developer key) is also required on requests\n    and is sent alongside `sessionId` in the appropriate header per BILL's\n    official reference.\n  sources:\n  - openapi/bill-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bill/refs/heads/main/authentication/bill-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Accounts Payable
- Accounts Receivable
- Spend Management
- Expense Management
- Payments
- Bill Pay
- Financial Operations
- Fintech
---
