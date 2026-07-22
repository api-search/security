---
api_key_in: []
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Miri Authentication
name_suffix: Authentication
oauth_flows: []
overview: Miri secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Miri
provider_slug: miri
scheme_count: 1
schemes:
- description: Per-account API key (API_KEY) used for server-side calls to the Miri API and to initialize the Miri Component SDK. Issued on developer-account registration.
  in: header
  name: apiKey
  sources:
  - https://www.miri.ai/developer/docs/alpha/main
  type: apiKey
slug: miri-authentication
source_filename: miri-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.miri.ai/developer/docs/alpha/main\ndocs: https://www.miri.ai/developer/docs/alpha/main\nsummary:\n  types:\n  - apiKey\n  notes: >-\n    Miri's developer program is in alpha. Server-side communication with the Miri API\n    uses a unique per-account API key (API_KEY) issued when a developer registers in\n    their Miri developer account. The React Native Component SDK is initialized with\n    the same key via its context provider. Webhooks are authenticated with API keys or\n    tokens per the integrator's security needs. No public OAuth or OpenID Connect flow\n    is documented at this alpha stage.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  description: >-\n    Per-account API key (API_KEY) used for server-side calls to the Miri API and to\n    initialize the Miri Component SDK. Issued on developer-account registration.\n  sources:\n  - https://www.miri.ai/developer/docs/alpha/main\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/miri/refs/heads/main/authentication/miri-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Health
- Wellness
- Digital Health
- Telehealth
- Artificial Intelligence
- Patient Engagement
- Weight Loss
- SDK
- Webhooks
---
