---
anonymous_access: false
api_key_in: []
api_specs:
- filename: surge-ai-projects-api-openapi.yml
  format: yaml
  label: Surge AI Projects API
  slug: surge-ai-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/surge-ai/openapi/surge-ai-projects-api-openapi.yml
- filename: surge-ai-tasks-api-openapi.yml
  format: yaml
  label: Surge AI Tasks API
  slug: surge-ai-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/surge-ai/openapi/surge-ai-tasks-api-openapi.yml
- filename: surge-ai-teams-api-openapi.yml
  format: yaml
  label: Surge AI Teams API
  slug: surge-ai-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/surge-ai/openapi/surge-ai-teams-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Surge Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Surge AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Surge AI
provider_slug: surge-ai
scheme_count: 1
schemes:
- description: HTTP Basic auth with the API key as username and an empty password (SDK sends auth=(api_key, "")). The key "is available in your Surge Profile"; the SDK reads it from surge.api_key or the SURGE_API_KEY environment variable.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/surge-ai-projects-api-openapi.yml
  - https://github.com/surge-ai/surge-python/blob/main/surge/api_resource.py
  - https://github.com/surge-ai/surge-python/blob/main/README.md
  type: http
slug: surge-ai-authentication
source_filename: surge-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: searched\nsource: https://github.com/surge-ai/surge-python/blob/main/README.md\ndocs: https://app.surgehq.ai/docs/api\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth with the API key as username and an empty password (SDK sends auth=(api_key, \"\")). The key\n    \"is available in your Surge Profile\"; the SDK reads it from surge.api_key or the SURGE_API_KEY environment variable.\n  sources:\n  - openapi/surge-ai-projects-api-openapi.yml\n  - https://github.com/surge-ai/surge-python/blob/main/surge/api_resource.py\n  - https://github.com/surge-ai/surge-python/blob/main/README.md\nnote: The API reference at app.surgehq.ai/docs/api redirects unauthenticated visitors to /customers/sign_in (checked 2026-10-27),\n  so the auth description is taken from the first-party SDK. Dashboard login also offers Google and SAML SSO; these are for\n  the web app, not the API.\n"
source_yaml_url: https://artifacts.apis.io/surge-ai/authentication/surge-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Human Data
- RLHF
- SFT
- Rubrics
- Verifiers
- RL Environments
- Multi-Modal
- Internationalization
- Labeling
---
