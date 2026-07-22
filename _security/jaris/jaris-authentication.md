---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Jaris Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jaris secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Jaris
provider_slug: jaris
scheme_count: 1
schemes:
- description: 'Jaris authenticates API integrations with an API key generated in the

    Jaris Dashboard. Documented on the Developer Overview; the full reference

    lives behind a password-protected ReadMe portal at docs.jaris.com, so this

    profile captures the model without a machine-readable securityScheme.

    '
  in: header
  name: apiKey
  sources:
  - https://jaris.io/developer-overview
  type: apiKey
slug: jaris-authentication
source_filename: jaris-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://jaris.io/developer-overview\ndocs: https://docs.jaris.com\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  description: |\n    Jaris authenticates API integrations with an API key generated in the\n    Jaris Dashboard. Documented on the Developer Overview; the full reference\n    lives behind a password-protected ReadMe portal at docs.jaris.com, so this\n    profile captures the model without a machine-readable securityScheme.\n  sources:\n  - https://jaris.io/developer-overview\nnotes: |\n  No public OpenAPI is available for Jaris (developer docs are gated), so this\n  authentication profile is searched from the public developer overview rather\n  than derived from a spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jaris/refs/heads/main/authentication/jaris-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Embedded Finance
- Fintech
- Payments
- Lending
- Banking as a Service
- Instant Payouts
- Merchant Onboarding
- KYB
- Settlements
---
