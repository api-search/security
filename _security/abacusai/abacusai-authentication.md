---
api_key_in:
- client
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Abacusai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Abacus.ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Abacus.ai
provider_slug: abacusai
scheme_count: 1
schemes:
- description: API key generated at https://abacus.ai/app/profile/apikey and passed to the ApiClient (Python client) or sent to the REST API. Within Abacus.AI hosted Notebooks the client initializes without an explicit key.
  in: client
  key_management: https://abacus.ai/app/profile/apikey
  name: ApiKey
  sources:
  - https://abacus.ai/help/python-sdk/getting-started
  - https://github.com/abacusai/api-python
  type: apiKey
slug: abacusai-authentication
source_filename: abacusai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://abacus.ai/help/python-sdk/getting-started\ndocs: https://abacus.ai/help/python-sdk/getting-started\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - client\n  oauth2_flows: []\n  notes: Authentication is via an API key generated from the Abacus.AI user profile\n    (https://abacus.ai/app/profile/apikey). The key is supplied to the first-party\n    Python client at construction time (ApiClient(api_key)); the SDK manages the API\n    key transport to the REST API internally. No OAuth2 / OpenID Connect flow is documented\n    for the platform REST API.\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: client\n  description: API key generated at https://abacus.ai/app/profile/apikey and passed\n    to the ApiClient (Python client) or sent to the REST API. Within Abacus.AI hosted\n    Notebooks the client initializes without an explicit key.\n  key_management: https://abacus.ai/app/profile/apikey\n  sources:\n  - https://abacus.ai/help/python-sdk/getting-started\n\
  \  - https://github.com/abacusai/api-python\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abacusai/refs/heads/main/authentication/abacusai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai Ml
- Artificial Intelligence
- Machine Learning
- Generative AI
- LLM
- AI Agents
- MLOps
- Enterprise AI
- Data Science
---
