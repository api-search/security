---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Einstein Vision API
  slug: einstein-vision-api
  spec_type: OpenAPI
  url: https://api.einstein.ai/v2/vision/openapi.json
- filename: openapi.json
  format: json
  label: Einstein Language API
  slug: einstein-language-api
  spec_type: OpenAPI
  url: https://api.einstein.ai/v2/language/openapi.json
- filename: salesforce-einstein-prediction-builder-openapi.yml
  format: yaml
  label: Einstein Prediction Builder API
  slug: einstein-prediction-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-prediction-builder-openapi.yml
- filename: salesforce-einstein-discovery-openapi.yml
  format: yaml
  label: Einstein Discovery API
  slug: einstein-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-discovery-openapi.yml
- filename: salesforce-einstein-bots-openapi.yml
  format: yaml
  label: Einstein Bots API
  slug: einstein-bots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-bots-openapi.yml
- filename: salesforce-einstein-gpt-openapi.yml
  format: yaml
  label: Einstein GPT API
  slug: einstein-gpt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-gpt-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Salesforce Einstein Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Salesforce Einstein secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Salesforce Einstein
provider_slug: salesforce-einstein
scheme_count: 2
schemes:
- description: Salesforce OAuth 2.0 authentication.
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  sources:
  - openapi/salesforce-einstein-bots-openapi.yml
  - openapi/salesforce-einstein-discovery-openapi.yml
  - openapi/salesforce-einstein-gpt-openapi.yml
  - openapi/salesforce-einstein-prediction-builder-openapi.yml
  type: oauth2
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token. Generate a token using your Einstein Platform Services private key.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/salesforce-einstein-language-openapi.yml
  - openapi/salesforce-einstein-vision-openapi.yml
  type: http
slug: salesforce-einstein-authentication
source_filename: salesforce-einstein-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesforce-einstein-bots-openapi.yml, openapi/salesforce-einstein-discovery-openapi.yml,\n  openapi/salesforce-einstein-gpt-openapi.yml, openapi/salesforce-einstein-language-openapi.yml,\n  openapi/salesforce-einstein-prediction-builder-openapi.yml, openapi/salesforce-einstein-vision-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n    scopes: 2\n  description: Salesforce OAuth 2.0 authentication.\n  sources:\n  - openapi/salesforce-einstein-bots-openapi.yml\n  - openapi/salesforce-einstein-discovery-openapi.yml\n  - openapi/salesforce-einstein-gpt-openapi.yml\n  - openapi/salesforce-einstein-prediction-builder-openapi.yml\n- name: bearerAuth\n  type:\
  \ http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token. Generate a token using your Einstein Platform Services\n    private key.\n  sources:\n  - openapi/salesforce-einstein-language-openapi.yml\n  - openapi/salesforce-einstein-vision-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/authentication/salesforce-einstein-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Artificial Intelligence
- Computer Vision
- CRM
- Machine Learning
- Natural Language Processing
- Predictive Analytics
- Salesforce
---
