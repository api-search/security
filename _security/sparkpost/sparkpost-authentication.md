---
api_key_in:
- header
api_specs:
- filename: sparkpost-transmissions-openapi.yml
  format: yaml
  label: SparkPost Transmissions API
  slug: transmissions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-transmissions-openapi.yml
- filename: sparkpost-templates-openapi.yml
  format: yaml
  label: SparkPost Templates API
  slug: templates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-templates-openapi.yml
- filename: sparkpost-metrics-openapi.yml
  format: yaml
  label: SparkPost Metrics API
  slug: metrics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-metrics-openapi.yml
- filename: sparkpost-events-openapi.yml
  format: yaml
  label: SparkPost Message Events API
  slug: events
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-events-openapi.yml
- filename: sparkpost-webhooks-openapi.yml
  format: yaml
  label: SparkPost Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-webhooks-openapi.yml
- filename: sparkpost-suppression-list-openapi.yml
  format: yaml
  label: SparkPost Suppression List API
  slug: suppression-list
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-suppression-list-openapi.yml
- filename: sparkpost-recipient-lists-openapi.yml
  format: yaml
  label: SparkPost Recipient Lists API
  slug: recipient-lists
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-recipient-lists-openapi.yml
- filename: sparkpost-sending-domains-openapi.yml
  format: yaml
  label: SparkPost Sending Domains API
  slug: sending-domains
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-sending-domains-openapi.yml
- filename: sparkpost-subaccounts-openapi.yml
  format: yaml
  label: SparkPost Subaccounts API
  slug: subaccounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-subaccounts-openapi.yml
- filename: sparkpost-inbound-openapi.yml
  format: yaml
  label: SparkPost Inbound Domains & Relay Webhooks API
  slug: inbound
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-inbound-openapi.yml
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
