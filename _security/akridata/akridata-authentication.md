---
api_key_in:
- config
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Akridata Authentication
name_suffix: Authentication
oauth_flows: []
overview: Akridata secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Akridata
provider_slug: akridata
scheme_count: 1
schemes:
- client_class: AkriDEClient
  config_docs: https://docs.akridata.ai/docs/download-config-saas
  description: 'Data Explorer authenticates SDK/CLI requests with an API key. The key is obtained by downloading the SDK configuration from the Data Explorer profile/UI, then supplied to the AkriDEClient (or the akride ingest CLI via -a) alongside the SaaS endpoint. Example config: {"saas_endpoint": "https://app.akridata.ai", "api_key": "<your-api-key>", "mode": "saas"}.'
  in: config
  name: apiKey
  saas_endpoint: https://app.akridata.ai
  sources:
  - https://pypi.org/project/akride/
  type: apiKey
slug: akridata-authentication
source_filename: akridata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://docs.akridata.ai/docs/download-config-saas\ndocs: https://docs.akridata.ai/docs/sdk-for-api-access\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - config\n  oauth2_flows: []\nschemes:\n- name: apiKey\n  type: apiKey\n  in: config\n  description: >-\n    Data Explorer authenticates SDK/CLI requests with an API key. The key is obtained\n    by downloading the SDK configuration from the Data Explorer profile/UI, then\n    supplied to the AkriDEClient (or the akride ingest CLI via -a) alongside the SaaS\n    endpoint. Example config: {\"saas_endpoint\": \"https://app.akridata.ai\",\n    \"api_key\": \"<your-api-key>\", \"mode\": \"saas\"}.\n  saas_endpoint: https://app.akridata.ai\n  client_class: AkriDEClient\n  config_docs: https://docs.akridata.ai/docs/download-config-saas\n  sources:\n  - https://pypi.org/project/akride/\nnotes: >-\n  No published OpenAPI/securitySchemes; derived from the published SDK quickstart\
  \ and\n  Data Explorer download-config documentation. No OAuth2/OIDC surface documented (API\n  key only), so scopes/ is intentionally skipped.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akridata/refs/heads/main/authentication/akridata-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Computer Vision
- Data Curation
- Machine Learning
- Visual Inspection
- Data Explorer
- MLOps
---
