---
api_key_in:
- header
api_specs:
- filename: goodstack-openapi-original.json
  format: json
  label: Goodstack Services
  slug: goodstack-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodstack/refs/heads/main/openapi/goodstack-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Goodstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Goodstack secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Goodstack
provider_slug: goodstack
scheme_count: 3
schemes:
- description: API key starting with 'pk_'. Identifies the Goodstack account; safe to expose in client-side code / SDKs.
  in: header
  name: PublishableApiKey
  parameter: Authorization
  sources:
  - openapi/goodstack-openapi-original.json
  type: apiKey
- description: API key starting with 'sk_'. Server-side only; must be kept secret.
  in: header
  name: SecretApiKey
  parameter: Authorization
  sources:
  - openapi/goodstack-openapi-original.json
  type: apiKey
- description: Scopes hosted donation-session requests.
  in: header
  name: DonationSessionToken
  parameter: donation-session-token
  sources:
  - openapi/goodstack-openapi-original.json
  type: apiKey
slug: goodstack-authentication
source_filename: goodstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.goodstack.io/docs/api/goodstack-services\ndocs: https://docs.goodstack.io/docs/api/goodstack-services\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: PublishableApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    API key starting with 'pk_'. Identifies the Goodstack account; safe to\n    expose in client-side code / SDKs.\n  sources: [openapi/goodstack-openapi-original.json]\n- name: SecretApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    API key starting with 'sk_'. Server-side only; must be kept secret.\n  sources: [openapi/goodstack-openapi-original.json]\n- name: DonationSessionToken\n  type: apiKey\n  in: header\n  parameter: donation-session-token\n  description: Scopes hosted donation-session requests.\n  sources: [openapi/goodstack-openapi-original.json]\nnotes:\n  - Keys are issued from\
  \ the Goodstack Partner dashboard.\n  - No OAuth 2.0 or OpenID Connect surface; there is no scope model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodstack/refs/heads/main/authentication/goodstack-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Nonprofits
- Donations
- Charitable Giving
- Fundraising
- Verification
- Compliance
- Payments
- Disbursements
- Social Impact
---
