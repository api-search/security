---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Kimola Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kimola secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kimola
provider_slug: kimola
scheme_count: 1
schemes:
- format: Bearer <apiKey>
  header: Authorization
  key_source: Kimola dashboard Account menu / Models page
  location: header
  name: bearerAuth
  scheme: bearer
  sources:
  - https://github.com/Kimola/api
  - https://github.com/Kimola/kimola-cognitive-api-documentation
  type: http
slug: kimola-authentication
source_filename: kimola-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/Kimola/api\ndocs: https://github.com/Kimola/api#authentication\nsummary:\n  types: [http]\n  scheme: bearer\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    The Kimola API authenticates with an API key presented as an HTTP Bearer\n    token in the Authorization header (Authorization: Bearer <apiKey>). The API\n    key is obtained from the Kimola dashboard Account menu (and the Models page\n    for the Cognitive API). Although the Cognitive documentation describes the\n    service as a \"JSON-based OAuth2 API\", no OAuth2 authorization/token flows or\n    scopes are documented; access is a static per-account bearer key. Key\n    validation is cached server-side for performance.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    location: header\n    header: Authorization\n    format: \"Bearer <apiKey>\"\n    key_source: Kimola dashboard Account menu / Models page\n    sources:\n\
  \      - https://github.com/Kimola/api\n      - https://github.com/Kimola/kimola-cognitive-api-documentation\nerrors:\n  - status: 400\n    when: Authorization header missing or not in Bearer format\n  - status: 401\n    when: The provided API key is invalid\n  - status: 403\n    when: The key lacks access to the requested resource/model\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kimola/refs/heads/main/authentication/kimola-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Market Research
- Customer Feedback
- Text Analytics
- Sentiment Analysis
- Natural Language Processing
- Consumer Insights
- Machine Learning
- Artificial Intelligence
---
