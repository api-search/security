---
api_key_in:
- header
api_specs:
- filename: sparkpost-dkim-keys-api-openapi.yml
  format: yaml
  label: SparkPost DKIM Keys API
  slug: sparkpost-dkim-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-dkim-keys-api-openapi.yml
- filename: sparkpost-events-api-openapi.yml
  format: yaml
  label: SparkPost Events API
  slug: sparkpost-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-events-api-openapi.yml
- filename: sparkpost-inbound-domains-api-openapi.yml
  format: yaml
  label: SparkPost Inbound Domains API
  slug: sparkpost-inbound-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-inbound-domains-api-openapi.yml
- filename: sparkpost-metrics-api-openapi.yml
  format: yaml
  label: SparkPost Metrics API
  slug: sparkpost-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-metrics-api-openapi.yml
- filename: sparkpost-recipient-lists-api-openapi.yml
  format: yaml
  label: SparkPost Recipient Lists API
  slug: sparkpost-recipient-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-recipient-lists-api-openapi.yml
- filename: sparkpost-relay-webhooks-api-openapi.yml
  format: yaml
  label: SparkPost Relay Webhooks API
  slug: sparkpost-relay-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-relay-webhooks-api-openapi.yml
- filename: sparkpost-sending-domains-api-openapi.yml
  format: yaml
  label: SparkPost Sending Domains API
  slug: sparkpost-sending-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-sending-domains-api-openapi.yml
- filename: sparkpost-subaccounts-api-openapi.yml
  format: yaml
  label: SparkPost Subaccounts API
  slug: sparkpost-subaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-subaccounts-api-openapi.yml
- filename: sparkpost-suppression-list-api-openapi.yml
  format: yaml
  label: SparkPost Suppression List API
  slug: sparkpost-suppression-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-suppression-list-api-openapi.yml
- filename: sparkpost-templates-api-openapi.yml
  format: yaml
  label: SparkPost Templates API
  slug: sparkpost-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-templates-api-openapi.yml
- filename: sparkpost-transmissions-api-openapi.yml
  format: yaml
  label: SparkPost Transmissions API
  slug: sparkpost-transmissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-transmissions-api-openapi.yml
- filename: sparkpost-webhooks-api-openapi.yml
  format: yaml
  label: SparkPost Webhooks API
  slug: sparkpost-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sparkpost Authentication
name_suffix: Authentication
oauth_flows: []
overview: SparkPost secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SparkPost
provider_slug: sparkpost
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/sparkpost-events-openapi.yml
  - openapi/sparkpost-inbound-openapi.yml
  - openapi/sparkpost-metrics-openapi.yml
  - openapi/sparkpost-recipient-lists-openapi.yml
  - openapi/sparkpost-sending-domains-openapi.yml
  - openapi/sparkpost-subaccounts-openapi.yml
  - openapi/sparkpost-suppression-list-openapi.yml
  - openapi/sparkpost-templates-openapi.yml
  - openapi/sparkpost-transmissions-openapi.yml
  - openapi/sparkpost-webhooks-openapi.yml
  type: apiKey
slug: sparkpost-authentication
source_filename: sparkpost-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sparkpost-events-openapi.yml, openapi/sparkpost-inbound-openapi.yml, openapi/sparkpost-metrics-openapi.yml,\n  openapi/sparkpost-recipient-lists-openapi.yml, openapi/sparkpost-sending-domains-openapi.yml,\n  openapi/sparkpost-subaccounts-openapi.yml, openapi/sparkpost-suppression-list-openapi.yml,\n  openapi/sparkpost-templates-openapi.yml, openapi/sparkpost-transmissions-openapi.yml, openapi/sparkpost-webhooks-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/sparkpost-events-openapi.yml\n  - openapi/sparkpost-inbound-openapi.yml\n  - openapi/sparkpost-metrics-openapi.yml\n  - openapi/sparkpost-recipient-lists-openapi.yml\n  - openapi/sparkpost-sending-domains-openapi.yml\n  - openapi/sparkpost-subaccounts-openapi.yml\n  - openapi/sparkpost-suppression-list-openapi.yml\n  - openapi/sparkpost-templates-openapi.yml\n\
  \  - openapi/sparkpost-transmissions-openapi.yml\n  - openapi/sparkpost-webhooks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/authentication/sparkpost-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Email
- Transactional Email
- Marketing Email
- Email Delivery
- SMTP
- Webhooks
- Analytics
- Templates
- Suppression List
---
