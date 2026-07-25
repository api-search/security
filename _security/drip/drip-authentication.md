---
api_key_in: []
api_specs:
- filename: drip-accounts-api-openapi.yml
  format: yaml
  label: Drip Accounts API
  slug: drip-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-accounts-api-openapi.yml
- filename: drip-broadcasts-api-openapi.yml
  format: yaml
  label: Drip Broadcasts API
  slug: drip-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-broadcasts-api-openapi.yml
- filename: drip-campaigns-api-openapi.yml
  format: yaml
  label: Drip Campaigns API
  slug: drip-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-campaigns-api-openapi.yml
- filename: drip-conversions-api-openapi.yml
  format: yaml
  label: Drip Conversions API
  slug: drip-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-conversions-api-openapi.yml
- filename: drip-custom-fields-api-openapi.yml
  format: yaml
  label: Drip Custom Fields API
  slug: drip-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-custom-fields-api-openapi.yml
- filename: drip-events-api-openapi.yml
  format: yaml
  label: Drip Events API
  slug: drip-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-events-api-openapi.yml
- filename: drip-forms-api-openapi.yml
  format: yaml
  label: Drip Forms API
  slug: drip-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-forms-api-openapi.yml
- filename: drip-orders-api-openapi.yml
  format: yaml
  label: Drip Orders API
  slug: drip-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-orders-api-openapi.yml
- filename: drip-shopper-activity-api-openapi.yml
  format: yaml
  label: Drip Shopper Activity API
  slug: drip-shopper-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-shopper-activity-api-openapi.yml
- filename: drip-subscribers-api-openapi.yml
  format: yaml
  label: Drip Subscribers API
  slug: drip-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-subscribers-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Drip Authentication
name_suffix: Authentication
oauth_flows: []
overview: Drip secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Drip
provider_slug: drip
scheme_count: 2
schemes:
- description: API token used as username with empty password
  name: basicAuth
  scheme: basic
  sources:
  - openapi/drip-openapi.yml
  type: http
- bearerFormat: OAuth2 access token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/drip-openapi.yml
  type: http
slug: drip-authentication
source_filename: drip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/drip-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: API token used as username with empty password\n  sources:\n  - openapi/drip-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2 access token\n  sources:\n  - openapi/drip-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/authentication/drip-authentication.yml
summary_line: http · 2 schemes
tags:
- Email Marketing
- Marketing Automation
- Ecommerce
- Customer Engagement
- Campaigns
- Workflows
---
