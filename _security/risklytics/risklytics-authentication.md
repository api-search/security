---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Risklytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Risklytics secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Risklytics
provider_slug: risklytics
scheme_count: 1
schemes:
- description: Personal API key issued per account through the platform dashboard.
  in: header
  name: apiKey
  sources:
  - https://www.risklytics.ai/pricing
  - https://www.risklytics.ai/docs
  type: apiKey
slug: risklytics-authentication
source_filename: risklytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.risklytics.ai/pricing\ndocs: https://www.risklytics.ai/docs\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  note: >-\n    Ember API access is authenticated with a personal API key issued through the signed-in platform\n    dashboard (platform.risklytics.ai). Request schemas, keys, usage, and billing live behind login;\n    no public OpenAPI or OAuth surface is published. Key placement (header) is documented in-platform;\n    recorded here as the conventional Authorization/API-key header pending a public spec.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  description: Personal API key issued per account through the platform dashboard.\n  sources: [https://www.risklytics.ai/pricing, https://www.risklytics.ai/docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/risklytics/refs/heads/main/authentication/risklytics-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Insurance
- InsurTech
- Risk
- Wildfire
- Property
- Catastrophe
- Analytics
- Machine Learning
- Underwriting
---
