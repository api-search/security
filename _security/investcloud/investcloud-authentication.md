---
api_key_in:
- unknown
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Investcloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: InvestCloud secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: InvestCloud
provider_slug: investcloud
scheme_count: 1
schemes:
- description: Per-application API keys issued and managed through the Wealthsqope Digital Developer portal's "stats and api keys" command center.
  gated: true
  in: unknown
  name: application-api-key
  parameter_name: unknown
  sources:
  - https://developer.investcloud.com/
  type: apiKey
slug: investcloud-authentication
source_filename: investcloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: https://developer.investcloud.com/\ndocs: https://developer.investcloud.com/\nnote: >-\n  DERIVED IS IMPOSSIBLE HERE — InvestCloud publishes no OpenAPI, so there are no securitySchemes to\n  aggregate. What IS knowable is stated on the public landing page of InvestCloud's own developer\n  portal, which advertises a \"stats and api keys\" command center to \"Track your api usage and\n  manage you application api keys\". That is a first-party statement that the platform authenticates\n  with per-application API keys. Everything else about the scheme — where the key travels (header,\n  query, or a signed envelope), its parameter name, key rotation, and whether OAuth is offered\n  alongside it — is behind the portal login and is recorded as unknown rather than guessed.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - unknown\n  oauth2_flows: []\n  confidence: low\n  basis: provider marketing copy on the public portal landing\
  \ page, not a specification\nschemes:\n- name: application-api-key\n  type: apiKey\n  in: unknown\n  parameter_name: unknown\n  description: >-\n    Per-application API keys issued and managed through the Wealthsqope Digital Developer portal's\n    \"stats and api keys\" command center.\n  sources:\n  - https://developer.investcloud.com/\n  gated: true\ngaps:\n- API key transport (header vs query vs body) is not publicly documented\n- no public statement on key rotation, expiry, or scoping\n- no evidence either way on OAuth 2.0 / OIDC support\n- no machine-readable securityScheme published anywhere\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/investcloud/refs/heads/main/authentication/investcloud-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Wealth Management
- Financial Services
- Investment Management
- WealthTech
- Portfolio Management
- Financial Planning
- Managed Accounts
- Advisor Technology
- Data Aggregation
---
