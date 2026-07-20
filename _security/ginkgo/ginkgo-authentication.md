---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Ginkgo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ginkgo Bioworks secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ginkgo Bioworks
provider_slug: ginkgo
scheme_count: 1
schemes:
- description: All requests to the Ginkgo AI Model API authenticate with a per-account API key passed in the `x-api-key` request header. Keys are issued (with usage credits) from the models portal at https://models.ginkgobioworks.ai/ and have the form xxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx. The official Python client reads the key from the GINKGOAI_API_KEY environment variable when not passed explicitly.
  env_var: GINKGOAI_API_KEY
  in: header
  key_format: xxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx
  name: ApiKeyAuth
  parameter_name: x-api-key
  registration_url: https://models.ginkgobioworks.ai/
  sources:
  - https://github.com/ginkgobioworks/ginkgo-ai-client
  type: apiKey
slug: ginkgo-authentication
source_filename: ginkgo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/ginkgobioworks/ginkgo-ai-client\ndocs: https://ginkgobioworks.github.io/ginkgo-ai-client/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  description: >-\n    All requests to the Ginkgo AI Model API authenticate with a per-account API\n    key passed in the `x-api-key` request header. Keys are issued (with usage\n    credits) from the models portal at https://models.ginkgobioworks.ai/ and\n    have the form xxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx. The official Python client\n    reads the key from the GINKGOAI_API_KEY environment variable when not passed\n    explicitly.\n  key_format: xxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx\n  env_var: GINKGOAI_API_KEY\n  registration_url: https://models.ginkgobioworks.ai/\n  sources:\n  - https://github.com/ginkgobioworks/ginkgo-ai-client\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ginkgo/refs/heads/main/authentication/ginkgo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Synthetic Biology
- Biotechnology
- Artificial Intelligence
- Machine Learning
- Protein Models
- Bioinformatics
- Inference API
---
