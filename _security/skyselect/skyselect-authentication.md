---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Skyselect Authentication
name_suffix: Authentication
oauth_flows: []
overview: SkySelect secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SkySelect
provider_slug: skyselect
scheme_count: 1
schemes:
- description: API Key and Secret pair generated in the SkySelect application under Settings > Developer Settings. Presented on API requests to authenticate integration partners (e.g. Rotabull) for inventory, RFQ, and quote flows.
  in: header
  name: apiKeyAndSecret
  sources:
  - https://support.rotabull.com/docs/skyselect
  type: apiKey
slug: skyselect-authentication
source_filename: skyselect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://support.rotabull.com/docs/skyselect\ndocs: https://help.skyselect.com/\nnote: >-\n  SkySelect exposes an API for buyer/supplier integrations (inventory sync, RFQ\n  reception, quote submission). Access is gated behind a login: credentials are\n  generated in the SkySelect app under Settings > Developer Settings. No public\n  OpenAPI or developer portal is published, so this profile is captured from the\n  provider Help Center and the Rotabull integration documentation.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: apiKeyAndSecret\n  type: apiKey\n  in: header\n  description: >-\n    API Key and Secret pair generated in the SkySelect application under\n    Settings > Developer Settings. Presented on API requests to authenticate\n    integration partners (e.g. Rotabull) for inventory, RFQ, and quote flows.\n  sources:\n  - https://support.rotabull.com/docs/skyselect\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skyselect/refs/heads/main/authentication/skyselect-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Marketplaces
- Aviation
- Procurement
- Supply Chain
- Aircraft Parts
- Artificial Intelligence
- MRO
---
