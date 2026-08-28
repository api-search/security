---
api_key_in:
- header
api_specs:
- filename: loudcrowd-openapi.yml
  format: yaml
  label: LoudCrowd Brand API
  slug: loudcrowd-brand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loudcrowd/refs/heads/main/openapi/loudcrowd-openapi.yml
- filename: loudcrowd-openapi.yml
  format: yaml
  label: LoudCrowd Attribution Events API
  slug: loudcrowd-attribution-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loudcrowd/refs/heads/main/openapi/loudcrowd-openapi.yml
- filename: loudcrowd-creator-storefronts-openapi.yml
  format: yaml
  label: LoudCrowd Creator Storefronts API
  slug: loudcrowd-creator-storefronts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loudcrowd/refs/heads/main/openapi/loudcrowd-creator-storefronts-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Loudcrowd Authentication
name_suffix: Authentication
oauth_flows: []
overview: LoudCrowd secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LoudCrowd
provider_slug: loudcrowd
scheme_count: 2
schemes:
- description: 'Authorization header using the Bearer scheme. Example: "Authorization: Bearer {token}"'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/loudcrowd-creator-storefronts-openapi.yml
  - openapi/loudcrowd-openapi.yml
  type: http
- description: API token created in LoudCrowd.
  in: header
  name: accountKeyAuth
  parameter: X-LC-Account-Key
  sources:
  - openapi/loudcrowd-openapi.yml
  type: apiKey
slug: loudcrowd-authentication
source_filename: loudcrowd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: derived\nsource: openapi/loudcrowd-creator-storefronts-openapi.yml, openapi/loudcrowd-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Authorization header using the Bearer scheme. Example: \"Authorization: Bearer\n    {token}\"'\n  sources:\n  - openapi/loudcrowd-creator-storefronts-openapi.yml\n  - openapi/loudcrowd-openapi.yml\n- name: accountKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-LC-Account-Key\n  description: API token created in LoudCrowd.\n  sources:\n  - openapi/loudcrowd-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loudcrowd/refs/heads/main/authentication/loudcrowd-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Creator Marketing
- Influencer Marketing
- Affiliate Marketing
- Ecommerce
- Creator Commerce
- Attribution
- Social Commerce
- Shopify
- User Generated Content
- Commissions
- Retail
- Marketing
---
