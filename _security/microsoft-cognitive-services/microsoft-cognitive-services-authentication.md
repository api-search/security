---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Cognitive Services Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Microsoft Cognitive Services secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Microsoft Cognitive Services
provider_slug: microsoft-cognitive-services
scheme_count: 2
schemes:
- description: Cognitive Services subscription key
  in: header
  name: subscription_key
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/microsoft-cognitive-services-openapi.yml
  type: apiKey
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: azure_auth
  sources:
  - openapi/microsoft-cognitive-services-openapi.yml
  type: oauth2
slug: microsoft-cognitive-services-authentication
source_filename: microsoft-cognitive-services-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-cognitive-services-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: subscription_key\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  description: Cognitive Services subscription key\n  sources:\n  - openapi/microsoft-cognitive-services-openapi.yml\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft Entra ID OAuth 2.0\n  sources:\n  - openapi/microsoft-cognitive-services-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-cognitive-services/refs/heads/main/authentication/microsoft-cognitive-services-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Azure AI
- Computer Vision
- Speech
- NLP
- OpenAI
- Machine Learning
---
