---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: mailbridgeapi-activity-api-openapi.yml
  format: yaml
  label: MailBridgeAPI Activity API
  slug: mailbridgeapi-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbridgeapi/openapi/mailbridgeapi-activity-api-openapi.yml
- filename: mailbridgeapi-compliance-api-openapi.yml
  format: yaml
  label: MailBridgeAPI Compliance API
  slug: mailbridgeapi-compliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbridgeapi/openapi/mailbridgeapi-compliance-api-openapi.yml
- filename: mailbridgeapi-mailbox-api-openapi.yml
  format: yaml
  label: MailBridgeAPI Mailbox API
  slug: mailbridgeapi-mailbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbridgeapi/openapi/mailbridgeapi-mailbox-api-openapi.yml
- filename: mailbridgeapi-receiving-api-openapi.yml
  format: yaml
  label: MailBridgeAPI Receiving API
  slug: mailbridgeapi-receiving-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbridgeapi/openapi/mailbridgeapi-receiving-api-openapi.yml
- filename: mailbridgeapi-sending-api-openapi.yml
  format: yaml
  label: MailBridgeAPI Sending API
  slug: mailbridgeapi-sending-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbridgeapi/openapi/mailbridgeapi-sending-api-openapi.yml
- filename: mailbridgeapi-service-api-openapi.yml
  format: yaml
  label: MailBridgeAPI Service API
  slug: mailbridgeapi-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbridgeapi/openapi/mailbridgeapi-service-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: derived
name: Mailbridgeapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: MailBridgeAPI secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MailBridgeAPI
provider_slug: mailbridgeapi
scheme_count: 4
schemes:
- description: 'Account API key. New endpoints also accept the value as an `Authorization: Bearer` token.'
  in: header
  name: AccountKey
  parameter: X-API-Key
  sources:
  - openapi/mailbridgeapi.json
  type: apiKey
- description: Mailbox API key selecting exactly one configured mailbox.
  in: header
  name: MailboxKey
  parameter: X-Mailbox-Key
  sources:
  - openapi/mailbridgeapi.json
  type: apiKey
- description: Account API key used by legacy-compatible endpoints. Prefer headers for new integrations when supported.
  in: query
  name: AccountKeyQuery
  parameter: apikey
  sources:
  - openapi/mailbridgeapi.json
  type: apiKey
- description: Mailbox API key used by legacy-compatible endpoints.
  in: query
  name: MailboxKeyQuery
  parameter: apikeybox
  sources:
  - openapi/mailbridgeapi.json
  type: apiKey
slug: mailbridgeapi-authentication
source_filename: mailbridgeapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: derived\nsource: openapi/mailbridgeapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: AccountKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'Account API key. New endpoints also accept the value as an `Authorization: Bearer`\n    token.'\n  sources:\n  - openapi/mailbridgeapi.json\n- name: MailboxKey\n  type: apiKey\n  in: header\n  parameter: X-Mailbox-Key\n  description: Mailbox API key selecting exactly one configured mailbox.\n  sources:\n  - openapi/mailbridgeapi.json\n- name: AccountKeyQuery\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: Account API key used by legacy-compatible endpoints. Prefer headers for new integrations\n    when supported.\n  sources:\n  - openapi/mailbridgeapi.json\n- name: MailboxKeyQuery\n  type: apiKey\n  in: query\n  parameter: apikeybox\n  description: Mailbox API key used by legacy-compatible endpoints.\n  sources:\n\
  \  - openapi/mailbridgeapi.json\n"
source_yaml_url: https://artifacts.apis.io/mailbridgeapi/authentication/mailbridgeapi-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Email API
- SMTP
- IMAP
- mailbox integration
- Developer Tools
- mailbox monitoring
---
