---
api_key_in: []
api_specs:
- filename: valimail-config-openapi-original.yml
  format: yaml
  label: Valimail Configuration API
  slug: valimail-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-config-openapi-original.yml
- filename: valimail-account-openapi-original.yml
  format: yaml
  label: Valimail Account Management API
  slug: valimail-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-account-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Valimail Authentication
name_suffix: Authentication
oauth_flows: []
overview: Valimail secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Valimail
provider_slug: valimail
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/valimail-account-openapi-original.yml
  - openapi/valimail-config-openapi-original.yml
  type: http
slug: valimail-authentication
source_filename: valimail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/valimail-account-openapi-original.yml, openapi/valimail-config-openapi-original.yml\ndocs: https://support.valimail.com/en/articles/10911168-api-authentication-and-authorization\nsummary:\n  types:\n  - http\n  flow: credential-exchange-to-bearer\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/valimail-account-openapi-original.yml\n  - openapi/valimail-config-openapi-original.yml\ncredential_exchange:\n  endpoint: POST https://api.valimail.com/auth\n  request: '{\"client-id\": \"...\", \"app-id\": \"...\"}'\n  response: '{\"token\": \"...\", \"expires-at\": \"ISO-8601 timestamp\"}'\n  usage: 'Authorization: Bearer <token> on all subsequent requests'\n  healthcheck: GET /healthcheck confirms API availability\nkey_management:\n  self_service: https://support.valimail.com/en/articles/11322142-api-key-self-service\n  notes: >-\n    API keys (Client ID + App ID)\
  \ are created in the Enforce app under Account\n    Settings -> API KEYS by Owner-type users; SSO or MFA must be enabled on the\n    account before keys can be created. Key access is scoped per API\n    (Configuration API, Reporting API, or both). Account Management API access\n    is granted to partners by Product Support. API access is included with\n    Enforce Enterprise and a paid add-on on Starter/Premium plans.\n  access_request: https://support.valimail.com/en/articles/10580387-requesting-api-access\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/authentication/valimail-authentication.yml
summary_line: http · 1 scheme
tags:
- Email Authentication
- DMARC
- Email Security
- SPF
- DKIM
- BIMI
- MTA-STS
- Anti-Phishing
- Deliverability
- Cybersecurity
---
