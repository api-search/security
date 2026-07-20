---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Ddd Invoices Authentication
name_suffix: Authentication
oauth_flows: []
overview: DDD Invoices secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DDD Invoices
provider_slug: ddd-invoices
scheme_count: 1
schemes:
- description: 'Custom token authentication. The Authorization header carries the literal scheme keyword "IoT" followed by the legal entity''s Connection Key and the target service name, e.g. "Authorization: IoT <connection-key>:EUeInvoices". HTTPS is required for all requests. TEST and PROD keys are distinct.'
  format: IoT <connection-key>:EUeInvoices
  in: header
  name: IoTConnectionKey
  parameter_name: Authorization
  sources:
  - https://dddinvoices.com/documentation-e-invoicing
  type: apiKey
slug: ddd-invoices-authentication
source_filename: ddd-invoices-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://dddinvoices.com/documentation-e-invoicing\ndocs: https://dddinvoices.com/documentation-e-invoicing\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  notes: >-\n    DDD Invoices uses a custom token (\"IoT\") scheme carried in the HTTP\n    Authorization header. There is no OAuth 2.0 / OpenID Connect surface\n    documented. A per-legal-entity Connection Key is issued after sign-up and\n    scopes calls to a service (EUeInvoices). Separate TEST and PROD connection\n    keys are provisioned per registered legal entity.\nschemes:\n- name: IoTConnectionKey\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  format: 'IoT <connection-key>:EUeInvoices'\n  description: >-\n    Custom token authentication. The Authorization header carries the literal\n    scheme keyword \"IoT\" followed by the legal entity's Connection Key and the\n    target service name, e.g. \"Authorization: IoT\
  \ <connection-key>:EUeInvoices\".\n    HTTPS is required for all requests. TEST and PROD keys are distinct.\n  sources:\n  - https://dddinvoices.com/documentation-e-invoicing\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ddd-invoices/refs/heads/main/authentication/ddd-invoices-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- e-Invoicing
- Fiscalization
- Tax Compliance
- Real-Time Reporting
- PEPPOL
- Invoicing
- API
---
