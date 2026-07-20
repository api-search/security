---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Aimon Authentication
name_suffix: Authentication
oauth_flows: []
overview: AIMon secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AIMon
provider_slug: aimon
scheme_count: 1
schemes:
- description: AIMon authenticates API and SDK calls with a Bearer API key. Sign up at app.aimon.ai, then go to My Account > Keys to copy your key. Provide it as the HTTP Authorization header in the form "Bearer <AIMON_API_KEY>". The SDKs read the key from the AIMON_API_KEY environment variable.
  env_var: AIMON_API_KEY
  header: Authorization
  header_format: Bearer <AIMON_API_KEY>
  key_management_url: https://app.aimon.ai/?screen=signup
  name: apiKey
  scheme: bearer
  sources:
  - https://docs.aimon.ai/quickstart
  - https://github.com/aimonlabs/aimon-python-sdk
  type: http
slug: aimon-authentication
source_filename: aimon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://docs.aimon.ai/quickstart\ndocs: https://docs.aimon.ai/quickstart\nsummary:\n  types: [http]\n  api_key_in: [header]\n  http_schemes: [bearer]\n  oauth2_flows: []\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: >-\n    AIMon authenticates API and SDK calls with a Bearer API key. Sign up at\n    app.aimon.ai, then go to My Account > Keys to copy your key. Provide it as the\n    HTTP Authorization header in the form \"Bearer <AIMON_API_KEY>\". The SDKs read the\n    key from the AIMON_API_KEY environment variable.\n  header: Authorization\n  header_format: Bearer <AIMON_API_KEY>\n  env_var: AIMON_API_KEY\n  key_management_url: https://app.aimon.ai/?screen=signup\n  sources: [https://docs.aimon.ai/quickstart, https://github.com/aimonlabs/aimon-python-sdk]\nnotes: >-\n  There is a key-validation endpoint (GET /v1/api-key/{api_key}/validate) exposed by\n  the API for verifying a key. No OAuth2 or\
  \ OpenID Connect flow is documented; auth is\n  a single long-lived Bearer API key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aimon/refs/heads/main/authentication/aimon-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai Ml
- LLM Observability
- AI Monitoring
- Evaluation
- Hallucination Detection
- LLM Guardrails
- RAG
- AI Governance
- Trustworthy AI
---
