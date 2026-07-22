---
api_key_in:
- body
- basic-auth-username
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Sift Science Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sift Science secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sift Science
provider_slug: sift-science
scheme_count: 2
schemes:
- applies_to:
  - Events API
  - Score API
  - Labels API
  in: body
  name: apiKeyBody
  parameter: api_key
  sources:
  - https://github.com/SiftScience/sift-python
  type: apiKey
- applies_to:
  - Decisions API
  - Workflow API
  - Verification API
  - PSP Merchant API
  description: HTTP Basic authentication with the API key as the username and an empty password.
  name: apiKeyBasic
  scheme: basic
  sources:
  - https://developers.sift.com/docs/curl/apis-overview
  type: http
slug: sift-science-authentication
source_filename: sift-science-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.sift.com/docs/curl/apis-overview\ndocs: https://developers.sift.com/docs/curl/apis-overview\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - body\n  - basic-auth-username\n  oauth2_flows: []\n  notes: >-\n    Sift authenticates every REST call with a per-account API key. For the Events, Score\n    and Labels APIs the API key is passed in the JSON request body as `api_key`. For the\n    Decisions, Workflow, Verification and other REST APIs the API key is supplied via HTTP\n    Basic authentication (the key is the Basic-auth username, password left blank). Many\n    endpoints additionally require the numeric `account_id`. Separate Sandbox and\n    Production API keys are issued per account from the Sift Console.\nschemes:\n- name: apiKeyBody\n  type: apiKey\n  in: body\n  parameter: api_key\n  applies_to:\n  - Events API\n  - Score API\n  - Labels API\n  sources:\n  - https://github.com/SiftScience/sift-python\n\
  - name: apiKeyBasic\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication with the API key as the username and an empty password.\n  applies_to:\n  - Decisions API\n  - Workflow API\n  - Verification API\n  - PSP Merchant API\n  sources:\n  - https://developers.sift.com/docs/curl/apis-overview\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sift-science/refs/heads/main/authentication/sift-science-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Enterprise Saas
- Fraud Detection
- Fraud Prevention
- Machine Learning
- Risk Scoring
- Payments
- Identity
- Security
- Digital Trust And Safety
---
