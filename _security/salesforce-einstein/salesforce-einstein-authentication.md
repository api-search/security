---
api_key_in: []
api_specs:
- filename: salesforce-einstein-ai-record-insights-api-openapi.yml
  format: yaml
  label: Salesforce Einstein AI Record Insights API
  slug: salesforce-einstein-ai-record-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-ai-record-insights-api-openapi.yml
- filename: salesforce-einstein-api-usage-api-openapi.yml
  format: yaml
  label: Salesforce Einstein API Usage API
  slug: salesforce-einstein-api-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-api-usage-api-openapi.yml
- filename: salesforce-einstein-bot-definitions-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Bot Definitions API
  slug: salesforce-einstein-bot-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-bot-definitions-api-openapi.yml
- filename: salesforce-einstein-bot-versions-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Bot Versions API
  slug: salesforce-einstein-bot-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-bot-versions-api-openapi.yml
- filename: salesforce-einstein-dashboards-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Dashboards API
  slug: salesforce-einstein-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-dashboards-api-openapi.yml
- filename: salesforce-einstein-datasets-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Datasets API
  slug: salesforce-einstein-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-datasets-api-openapi.yml
- filename: salesforce-einstein-examples-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Examples API
  slug: salesforce-einstein-examples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-examples-api-openapi.yml
- filename: salesforce-einstein-feedback-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Feedback API
  slug: salesforce-einstein-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-feedback-api-openapi.yml
- filename: salesforce-einstein-generations-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Generations API
  slug: salesforce-einstein-generations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-generations-api-openapi.yml
- filename: salesforce-einstein-lenses-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Lenses API
  slug: salesforce-einstein-lenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-lenses-api-openapi.yml
- filename: salesforce-einstein-messages-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Messages API
  slug: salesforce-einstein-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-messages-api-openapi.yml
- filename: salesforce-einstein-models-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Models API
  slug: salesforce-einstein-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-models-api-openapi.yml
- filename: salesforce-einstein-prediction-definitions-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Prediction Definitions API
  slug: salesforce-einstein-prediction-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-prediction-definitions-api-openapi.yml
- filename: salesforce-einstein-predictions-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Predictions API
  slug: salesforce-einstein-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-predictions-api-openapi.yml
- filename: salesforce-einstein-prompt-templates-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Prompt Templates API
  slug: salesforce-einstein-prompt-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-prompt-templates-api-openapi.yml
- filename: salesforce-einstein-sessions-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Sessions API
  slug: salesforce-einstein-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-sessions-api-openapi.yml
- filename: salesforce-einstein-stories-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Stories API
  slug: salesforce-einstein-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-stories-api-openapi.yml
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
- Computer-Vision
- CRM
- Machine-Learning
- Natural Language Processing
- Predictive Analytics
- Salesforce
---
