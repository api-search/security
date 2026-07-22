---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Emtech Authentication
name_suffix: Authentication
oauth_flows: []
overview: EMTECH secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: EMTECH
provider_slug: emtech
scheme_count: 1
schemes:
- environments:
  - test
  - live
  in: header
  issued_from: https://app.emtech.com
  name: apiKey
  sources:
  - https://developer.emtech.com/quickstart
  type: apiKey
slug: emtech-authentication
source_filename: emtech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.emtech.com/quickstart\ndocs: https://developer.emtech.com/quickstart\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  notes: >-\n    EMTECH APIs authenticate with an organization API key. Credentials are\n    unique to each organization and environment (Test or Live) and are issued\n    from the platform at https://app.emtech.com. A key grants access to\n    EMTECH's authentication, event-reporting, and compliance-workflow\n    endpoints. No public OpenAPI specification is published, so the header\n    name and key format below are described in the docs rather than derived\n    from a machine-readable spec.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  environments:\n  - test\n  - live\n  issued_from: https://app.emtech.com\n  sources:\n  - https://developer.emtech.com/quickstart\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emtech/refs/heads/main/authentication/emtech-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Financial Services
- Regtech
- Central Banking
- CBDC
- Digital Currency
- Compliance
- Regulatory Reporting
- Fintech
- Payments
---
