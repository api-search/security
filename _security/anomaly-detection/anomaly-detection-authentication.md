---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Anomaly Detection Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anomaly Detection secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Anomaly Detection
provider_slug: anomaly-detection
scheme_count: 1
schemes:
- description: Azure Cognitive Services subscription key for the Anomaly Detector resource.
  in: header
  name: SubscriptionKey
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/anomaly-detection-openapi.yml
  type: apiKey
slug: anomaly-detection-authentication
source_filename: anomaly-detection-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/anomaly-detection-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SubscriptionKey\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  description: Azure Cognitive Services subscription key for the Anomaly Detector resource.\n  sources:\n  - openapi/anomaly-detection-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anomaly-detection/refs/heads/main/authentication/anomaly-detection-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Anomaly Detection
- Artificial Intelligence
- Data Science
- Fraud Detection
- Machine Learning
- Monitoring
- Observability
- Outlier Detection
- Pattern Recognition
- Security
- Time Series
---
