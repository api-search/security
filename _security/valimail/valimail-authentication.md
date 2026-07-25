---
api_key_in: []
api_specs:
- filename: valimail-accounts-api-openapi.yml
  format: yaml
  label: Valimail Accounts API
  slug: valimail-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-accounts-api-openapi.yml
- filename: valimail-authentication-api-openapi.yml
  format: yaml
  label: Valimail Authentication API
  slug: valimail-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-authentication-api-openapi.yml
- filename: valimail-dkims-by-domain-api-openapi.yml
  format: yaml
  label: Valimail DKIMs by Domain API
  slug: valimail-dkims-by-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-dkims-by-domain-api-openapi.yml
- filename: valimail-dkims-by-sender-api-openapi.yml
  format: yaml
  label: Valimail DKIMs by Sender API
  slug: valimail-dkims-by-sender-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-dkims-by-sender-api-openapi.yml
- filename: valimail-domains-api-openapi.yml
  format: yaml
  label: Valimail Domains API
  slug: valimail-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-domains-api-openapi.yml
- filename: valimail-mta-sts-policy-api-openapi.yml
  format: yaml
  label: Valimail MTA-STS Policy API
  slug: valimail-mta-sts-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-mta-sts-policy-api-openapi.yml
- filename: valimail-mta-sts-policy-reports-api-openapi.yml
  format: yaml
  label: Valimail MTA-STS Policy Reports API
  slug: valimail-mta-sts-policy-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-mta-sts-policy-reports-api-openapi.yml
- filename: valimail-netblocks-api-openapi.yml
  format: yaml
  label: Valimail Netblocks API
  slug: valimail-netblocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-netblocks-api-openapi.yml
- filename: valimail-portfolios-api-openapi.yml
  format: yaml
  label: Valimail Portfolios API
  slug: valimail-portfolios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-portfolios-api-openapi.yml
- filename: valimail-scim-api-openapi.yml
  format: yaml
  label: Valimail SCIM API
  slug: valimail-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-scim-api-openapi.yml
- filename: valimail-senders-api-openapi.yml
  format: yaml
  label: Valimail Senders API
  slug: valimail-senders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-senders-api-openapi.yml
- filename: valimail-sso-api-openapi.yml
  format: yaml
  label: Valimail SSO API
  slug: valimail-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-sso-api-openapi.yml
- filename: valimail-tls-configuration-api-openapi.yml
  format: yaml
  label: Valimail TLS Configuration API
  slug: valimail-tls-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-tls-configuration-api-openapi.yml
- filename: valimail-users-api-openapi.yml
  format: yaml
  label: Valimail Users API
  slug: valimail-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-users-api-openapi.yml
- filename: valimail-webhooks-api-openapi.yml
  format: yaml
  label: Valimail Webhooks API
  slug: valimail-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-webhooks-api-openapi.yml
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
