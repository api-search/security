---
api_key_in:
- header
api_specs:
- filename: heron-webhooks-asyncapi.yml
  format: yaml
  label: Heron API
  slug: heron-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/heron/refs/heads/main/asyncapi/heron-webhooks-asyncapi.yml
auth_types:
- apiKey
description: 'Heron authenticates every API request with a customer-issued API key sent in the x-api-key HTTP header. Keys are managed from the dashboard (Settings -> API Credentials): create, list, deactivate, reactivate, delete, and rotate. Development and production are separated at the credential level — trial / onboarding uses development credentials, and production credentials are issued separately on request. A second key class, the "broker API key", authenticates the broker-submission endpoints and is generated per broker-funder relationship via /api/broker_submissions/api_keys/generate.'
kind: authentication
layout: security
method: searched
name: Heron Authentication
name_suffix: Authentication
oauth_flows: []
overview: Heron secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Heron
provider_slug: heron
scheme_count: 2
schemes:
- in: header
  key_format: key_ followed by 48 hexadecimal characters
  name: ApiKeyAuth
  parameter_name: x-api-key
  sources:
  - https://docs.herondata.io/api-reference/authentication
  token_visibility: Full token shown once at creation; only the first 8 characters (prefix) are retrievable afterwards.
  type: apiKey
- generation: POST /api/broker_submissions/api_keys/generate
  in: header
  name: BrokerApiKeyAuth
  parameter_name: x-api-key
  scope: broker-submission endpoints only
  sources:
  - https://docs.herondata.io/api-reference/brokersubmissions/generate-broker-api-key.md
  type: apiKey
slug: heron-authentication
source_filename: heron-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.herondata.io/api-reference/authentication\ndocs: https://docs.herondata.io/api-reference/authentication\ndescription: >-\n  Heron authenticates every API request with a customer-issued API key sent in\n  the x-api-key HTTP header. Keys are managed from the dashboard (Settings ->\n  API Credentials): create, list, deactivate, reactivate, delete, and rotate.\n  Development and production are separated at the credential level — trial /\n  onboarding uses development credentials, and production credentials are issued\n  separately on request. A second key class, the \"broker API key\", authenticates\n  the broker-submission endpoints and is generated per broker-funder\n  relationship via /api/broker_submissions/api_keys/generate.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter_name: x-api-key\n    key_format: key_\
  \ followed by 48 hexadecimal characters\n    token_visibility: >-\n      Full token shown once at creation; only the first 8 characters (prefix)\n      are retrievable afterwards.\n    sources: [https://docs.herondata.io/api-reference/authentication]\n  - name: BrokerApiKeyAuth\n    type: apiKey\n    in: header\n    parameter_name: x-api-key\n    scope: broker-submission endpoints only\n    generation: POST /api/broker_submissions/api_keys/generate\n    sources: [https://docs.herondata.io/api-reference/brokersubmissions/generate-broker-api-key.md]\nenvironments:\n  development: Issued for trial / onboarding; separated from production at the credential level.\n  production: Issued separately on request (contact your Heron rep / hello@herondata.io).\nrejected_status: 401 (deactivated or invalid key)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heron/refs/heads/main/authentication/heron-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Financial Services
- Document Automation
- Underwriting
- Lending
- Cashflow Analytics
- Fintech
- Data Enrichment
---
