---
api_key_in:
- environment-variable
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Symbolica Authentication
name_suffix: Authentication
oauth_flows: []
overview: Symbolica secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Symbolica
provider_slug: symbolica
scheme_count: 1
schemes:
- env_vars:
  - AGENTICA_API_KEY
  - NEXT_PUBLIC_AGENTICA_API_KEY
  - VITE_AGENTICA_API_KEY
  in: environment-variable
  name: AgenticaApiKey
  obtain: https://www.symbolica.ai/login
  scheme_detail: Agentica Platform API key supplied to the SDK via an environment variable. The SDK reads the key from the environment at runtime and authenticates to the Symbolica Platform (inference, sandboxing, hosting, observability) on the developer's behalf.
  signup_credits: New accounts receive $50 in free inference credits.
  type: apiKey
slug: symbolica-authentication
source_filename: symbolica-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.symbolica.ai/quickstart\ndocs: https://docs.symbolica.ai/quickstart\nsummary:\n  types: [apiKey]\n  api_key_in: [environment-variable]\n  oauth2_flows: []\nschemes:\n  - name: AgenticaApiKey\n    type: apiKey\n    in: environment-variable\n    scheme_detail: >-\n      Agentica Platform API key supplied to the SDK via an environment variable. The SDK\n      reads the key from the environment at runtime and authenticates to the Symbolica\n      Platform (inference, sandboxing, hosting, observability) on the developer's behalf.\n    env_vars:\n      - AGENTICA_API_KEY            # plain TS/JS, Python, and Bun\n      - NEXT_PUBLIC_AGENTICA_API_KEY # Next.js\n      - VITE_AGENTICA_API_KEY        # Vite + React\n    obtain: https://www.symbolica.ai/login\n    signup_credits: New accounts receive $50 in free inference credits.\nnotes: >-\n  Agentica is an SDK-first platform; authentication is a single platform API key\
  \ consumed by\n  the SDK rather than per-request HTTP auth headers documented on a REST surface. No OAuth2 /\n  OpenID Connect flows are published, so there is no scopes surface (scopes/ intentionally omitted).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/symbolica/refs/heads/main/authentication/symbolica-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Agents
- Agentic AI
- SDK
- Developer Tools
- LLM
- Machine Learning
---
