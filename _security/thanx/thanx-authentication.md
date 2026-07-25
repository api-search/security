---
api_key_in:
- header
api_specs:
- filename: thanx-account-api-openapi.yml
  format: yaml
  label: Thanx Account API
  slug: thanx-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-account-api-openapi.yml
- filename: thanx-auth-api-openapi.yml
  format: yaml
  label: Thanx Auth API
  slug: thanx-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-auth-api-openapi.yml
- filename: thanx-baskets-api-openapi.yml
  format: yaml
  label: Thanx Baskets API
  slug: thanx-baskets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-baskets-api-openapi.yml
- filename: thanx-campaigns-api-openapi.yml
  format: yaml
  label: Thanx Campaigns API
  slug: thanx-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-campaigns-api-openapi.yml
- filename: thanx-cards-api-openapi.yml
  format: yaml
  label: Thanx Cards API
  slug: thanx-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-cards-api-openapi.yml
- filename: thanx-gift-cards-api-openapi.yml
  format: yaml
  label: Thanx Gift Cards API
  slug: thanx-gift-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-gift-cards-api-openapi.yml
- filename: thanx-issuance-jobs-api-openapi.yml
  format: yaml
  label: Thanx Issuance Jobs API
  slug: thanx-issuance-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-issuance-jobs-api-openapi.yml
- filename: thanx-locations-api-openapi.yml
  format: yaml
  label: Thanx Locations API
  slug: thanx-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-locations-api-openapi.yml
- filename: thanx-metadata-api-openapi.yml
  format: yaml
  label: Thanx Metadata API
  slug: thanx-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-metadata-api-openapi.yml
- filename: thanx-points-api-openapi.yml
  format: yaml
  label: Thanx Points API
  slug: thanx-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-points-api-openapi.yml
- filename: thanx-purchases-api-openapi.yml
  format: yaml
  label: Thanx Purchases API
  slug: thanx-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-purchases-api-openapi.yml
- filename: thanx-rewards-api-openapi.yml
  format: yaml
  label: Thanx Rewards API
  slug: thanx-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-rewards-api-openapi.yml
- filename: thanx-subscribers-api-openapi.yml
  format: yaml
  label: Thanx Subscribers API
  slug: thanx-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-subscribers-api-openapi.yml
- filename: thanx-users-api-openapi.yml
  format: yaml
  label: Thanx Users API
  slug: thanx-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-users-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Thanx Authentication
name_suffix: Authentication
oauth_flows: []
overview: Thanx secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Thanx
provider_slug: thanx
scheme_count: 3
schemes:
- description: End-user access token acquired through Thanx SSO.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/thanx-consumer-api-openapi.yml
  - openapi/thanx-loyalty-api-openapi.yml
  - openapi/thanx-partner-api-openapi.yml
  type: http
- description: Client-specific identifier provided by Thanx.
  in: header
  name: clientId
  parameter: X-ClientId
  sources:
  - openapi/thanx-consumer-api-openapi.yml
  - openapi/thanx-partner-api-openapi.yml
  type: apiKey
- description: Merchant key provided by Thanx.
  in: header
  name: merchantKey
  parameter: Merchant-Key
  sources:
  - openapi/thanx-loyalty-api-openapi.yml
  type: apiKey
slug: thanx-authentication
source_filename: thanx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/thanx-consumer-api-openapi.yml, openapi/thanx-loyalty-api-openapi.yml, openapi/thanx-partner-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: End-user access token acquired through Thanx SSO.\n  sources:\n  - openapi/thanx-consumer-api-openapi.yml\n  - openapi/thanx-loyalty-api-openapi.yml\n  - openapi/thanx-partner-api-openapi.yml\n- name: clientId\n  type: apiKey\n  in: header\n  parameter: X-ClientId\n  description: Client-specific identifier provided by Thanx.\n  sources:\n  - openapi/thanx-consumer-api-openapi.yml\n  - openapi/thanx-partner-api-openapi.yml\n- name: merchantKey\n  type: apiKey\n  in: header\n  parameter: Merchant-Key\n  description: Merchant key provided by Thanx.\n  sources:\n  - openapi/thanx-loyalty-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/authentication/thanx-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Restaurant
- Loyalty
- Guest Engagement
- Marketing
- CRM
- Online Ordering
- Webhooks
- Points
- Rewards
- Campaigns
---
