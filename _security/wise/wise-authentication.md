---
api_key_in: []
api_specs:
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Profiles API
  slug: profiles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Recipients API
  slug: recipients
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Quotes API
  slug: quotes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Transfers API
  slug: transfers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Balances API
  slug: balances
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Multi-Currency Account API
  slug: multi-currency-account
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Statements API
  slug: statements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Cards API
  slug: cards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Simulation API
  slug: simulation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wise secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Wise
provider_slug: wise
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'User Access Token for making API calls on behalf of a Wise user.


    Can be obtained via two OAuth 2.0 flows:

    - **registration_code grant**: For partners creating users via API

    - **authorization_code grant**: For partners using Wise''s authorization page


    Access tokens are valid for 12 hours and can be refreshed using a refresh token.'
  name: UserToken
  scheme: bearer
  sources:
  - openapi/wise-platform-openapi.yml
  type: http
- description: 'Basic Authentication using your Client ID and Client Secret as the username and password.


    Client credentials are provided by Wise when your partnership begins. See [Getting Started](/guides/developer) for details.'
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/wise-platform-openapi.yml
  type: http
slug: wise-authentication
source_filename: wise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wise-platform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: UserToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    User Access Token for making API calls on behalf of a Wise user.\n\n    Can be obtained via two OAuth 2.0 flows:\n    - **registration_code grant**: For partners creating users via API\n    - **authorization_code grant**: For partners using Wise's authorization page\n\n    Access tokens are valid for 12 hours and can be refreshed using a refresh token.\n  sources:\n  - openapi/wise-platform-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: |-\n    Basic Authentication using your Client ID and Client Secret as the username and password.\n\n    Client credentials are provided by Wise when your partnership begins. See [Getting Started](/guides/developer) for details.\n  sources:\n  - openapi/wise-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/authentication/wise-authentication.yml
summary_line: http · 2 schemes
tags:
- Payments
- FX
- Cross-Border
- Banking
- Multi-Currency
---
