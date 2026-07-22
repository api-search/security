---
api_key_in:
- env
auth_types:
- apiKey
- http-bearer-jwt
description: Sphinx authenticates developers to its platform two ways. No public OpenAPI is published, so this profile is searched from the docs rather than derived from a spec.
kind: authentication
layout: security
method: searched
name: Sphinx Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sphinx secures its APIs with apiKey and http-bearer-jwt across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sphinx
provider_slug: sphinx
scheme_count: 2
schemes:
- description: API key obtained from the Sphinx Dashboard account settings. Stored in the SPHINX_API_KEY environment variable; the CLI uses it automatically when set, bypassing interactive login.
  env_var: SPHINX_API_KEY
  in: env
  name: ApiKey
  obtain: https://dashboard.prod.sphinx.ai
  prefix: sk-
  sources:
  - https://docs.sphinx.ai/cli-documentation/authentication
  type: apiKey
- bearerFormat: JWT
  description: Interactive login via `sphinx-cli auth login`, which persists a token in a ~/.sphinx directory. Token must be renewed every 30 days.
  name: JWTLogin
  scheme: bearer
  sources:
  - https://docs.sphinx.ai/cli-documentation/authentication
  type: http
slug: sphinx-authentication
source_filename: sphinx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.sphinx.ai/cli-documentation/authentication\ndocs: https://docs.sphinx.ai/cli-documentation/authentication\ndescription: >-\n  Sphinx authenticates developers to its platform two ways. No public OpenAPI is\n  published, so this profile is searched from the docs rather than derived from a\n  spec.\nsummary:\n  types: [apiKey, http-bearer-jwt]\n  api_key_in: [env]\n  api_key_prefix: \"sk-\"\nschemes:\n  - name: ApiKey\n    type: apiKey\n    in: env\n    env_var: SPHINX_API_KEY\n    prefix: \"sk-\"\n    description: >-\n      API key obtained from the Sphinx Dashboard account settings. Stored in the\n      SPHINX_API_KEY environment variable; the CLI uses it automatically when set,\n      bypassing interactive login.\n    obtain: https://dashboard.prod.sphinx.ai\n    sources: [https://docs.sphinx.ai/cli-documentation/authentication]\n  - name: JWTLogin\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n  \
  \  description: >-\n      Interactive login via `sphinx-cli auth login`, which persists a token in a\n      ~/.sphinx directory. Token must be renewed every 30 days.\n    sources: [https://docs.sphinx.ai/cli-documentation/authentication]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sphinx/refs/heads/main/authentication/sphinx-authentication.yml
summary_line: apiKey/http-bearer-jwt · 2 schemes
tags:
- Company
- Artificial Intelligence
- Data Science
- Data Governance
- Analytics
- AI Agents
- Developer Tools
- Jupyter
- LLM
- Data Reliability
---
