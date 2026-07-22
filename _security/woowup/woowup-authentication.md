---
api_key_in:
- header
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Woowup Authentication
name_suffix: Authentication
oauth_flows: []
overview: WoowUp secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: WoowUp
provider_slug: woowup
scheme_count: 2
schemes:
- format: 'Authorization: Basic {apikey}'
  in: header
  name: apikeyHeader
  notes: 'The docs'' recommended method sends the raw account API key after the Basic keyword (not base64 user:pass). Rate-limiting code examples also show ''Authorization: Bearer {api_token}'' accepted.'
  parameter: Authorization
  recommended: true
  type: apiKey
- format: ?apikey={apikey}
  in: query
  name: apikeyQuery
  parameter: apikey
  recommended: false
  type: apiKey
slug: woowup-authentication
source_filename: woowup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://woowup-docs.gitbook.io/woowup-developer-docs/master#authentication\nsource: >-\n  https://woowup-docs.gitbook.io/woowup-developer-docs/master (Getting Started,\n  Authentication section) and connection-security page. WoowUp publishes no\n  OpenAPI, so this profile is captured from the docs rather than derived from\n  securitySchemes.\nsummary:\n  types: [apiKey]\n  api_key_in: [header, query]\n  oauth2_flows: []\nschemes:\n  - name: apikeyHeader\n    type: apiKey\n    in: header\n    parameter: Authorization\n    format: 'Authorization: Basic {apikey}'\n    recommended: true\n    notes: >-\n      The docs' recommended method sends the raw account API key after the\n      Basic keyword (not base64 user:pass). Rate-limiting code examples also\n      show 'Authorization: Bearer {api_token}' accepted.\n  - name: apikeyQuery\n    type: apiKey\n    in: query\n    parameter: apikey\n    format: '?apikey={apikey}'\n    recommended:\
  \ false\nkey_management:\n  issuance: Log into WoowUp and get the API key from the Configuration / My Account section (app.woowup.com).\n  revocation: >-\n    Requests from deleted accounts receive HTTP 410 Gone with code\n    account_deleted; a deactivated account's API key is permanently invalid.\ntransport:\n  https_only: true\n  tls_minimum: '1.2'\n  docs: https://woowup-docs.gitbook.io/woowup-developer-docs/connection-security\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/woowup/refs/heads/main/authentication/woowup-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- CRM
- Loyalty
- Customer Data
- Marketing Automation
- Retail
- eCommerce
- Push Notifications
---
