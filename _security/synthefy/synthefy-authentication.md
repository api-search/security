---
api_key_in:
- header
- environment
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Synthefy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Synthefy secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Synthefy
provider_slug: synthefy
scheme_count: 2
schemes:
- description: Synthefy Forecasting API key supplied by the synthefy Python client (SynthefyAPIClient); set in code or via SYNTHEFY_API_KEY.
  in: header
  name: SynthefyApiKey
  scope: forecasting-api
  sources:
  - https://docs.synthefy.com/setup/api_key
  type: apiKey
- description: 'Nori hosted inference is called with an Authorization: Bearer $SYNTHEFY_NORI_API_KEY header against the OpenAI-style /predict endpoint.'
  name: NoriBearerToken
  scheme: bearer
  scope: nori
  sources:
  - https://docs.synthefy.com/nori/quickstart
  type: http
slug: synthefy-authentication
source_filename: synthefy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.synthefy.com/setup/api_key\ndocs: https://docs.synthefy.com/setup/api_key\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header, environment]\n  oauth2_flows: []\nnotes: >-\n  Synthefy authenticates with account API keys created in the Synthefy Console\n  (https://console.synthefy.com/, Settings -> API Keys). Keys can be passed to the\n  Python SDK via the api_key argument or the SYNTHEFY_API_KEY environment variable.\n  The classical Forecasting product and the Nori model use SEPARATE keys with\n  different rate limits and creation flows; a classical key does not authenticate\n  Nori requests. Nori allows exactly one key per account (shown once at creation,\n  not retrievable) and requires an active subscription.\nschemes:\n- name: SynthefyApiKey\n  type: apiKey\n  in: header\n  scope: forecasting-api\n  description: >-\n    Synthefy Forecasting API key supplied by the synthefy Python client\n    (SynthefyAPIClient);\
  \ set in code or via SYNTHEFY_API_KEY.\n  sources: [https://docs.synthefy.com/setup/api_key]\n- name: NoriBearerToken\n  type: http\n  scheme: bearer\n  scope: nori\n  description: >-\n    Nori hosted inference is called with an Authorization: Bearer\n    $SYNTHEFY_NORI_API_KEY header against the OpenAI-style /predict endpoint.\n  sources: [https://docs.synthefy.com/nori/quickstart]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synthefy/refs/heads/main/authentication/synthefy-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Foundation Models
- Machine Learning
- Forecasting
- Time Series
- Tabular Data
- Synthetic Data
- Artificial Intelligence
- Predictive Analytics
---
