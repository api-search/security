---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Boosted Authentication
name_suffix: Authentication
oauth_flows: []
overview: Boosted.ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Boosted.ai
provider_slug: boosted
scheme_count: 1
schemes:
- description: 'Boosted.ai (Alfa) API requests authenticate with an API key passed in the x-api-key request header, as shown in the provider''s published Python example (headers = {"x-api-key": API_KEY}). Keys are issued per client.'
  in: header
  name: apiKey
  parameter_name: x-api-key
  sources:
  - https://www.boosted.ai/api
  type: apiKey
slug: boosted-authentication
source_filename: boosted-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.boosted.ai/api\ndocs: https://www.boosted.ai/api\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  description: >-\n    Boosted.ai (Alfa) API requests authenticate with an API key passed in the\n    x-api-key request header, as shown in the provider's published Python\n    example (headers = {\"x-api-key\": API_KEY}). Keys are issued per client.\n  sources: [https://www.boosted.ai/api]\nnotes: >-\n  No public OpenAPI/Swagger specification is published for the Boosted.ai API;\n  the auth model is captured from the provider's documented API code sample.\n  The application host (alfa-3.boosted.ai) additionally fronts an OIDC/OAuth\n  login surface for the web app, but the developer API itself is API-key based.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boosted/refs/heads/main/authentication/boosted-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Finance
- Investment Management
- Financial Services
- Agents
- Machine Learning
- Research
- Fintech
---
