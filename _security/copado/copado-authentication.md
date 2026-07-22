---
api_key_in:
- header
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Copado Authentication
name_suffix: Authentication
oauth_flows: []
overview: Copado secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Copado
provider_slug: copado
scheme_count: 1
schemes:
- description: 'Copado APIs (Actions API, Webhooks API) are authenticated with a Copado API key.

    Users generate/reset the key from the Copado Account Summary > API Key tab; the key

    is passed as a parameter on webhook/action callout URLs. Copado Essentials issues a

    per-account API token used the same way.

    '
  docs: https://docs.essentials.copado.com/en/articles/6808604-copado-essentials-api-token
  in: query
  key: api_key
  name: ApiKey
  type: apiKey
slug: copado-authentication
source_filename: copado-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.copado.com/developer-hub + https://copadomulticoudwebhooks.docs.apiary.io/ + https://docs.essentials.copado.com/en/articles/6808604-copado-essentials-api-token\nsummary:\n  types: [apiKey]\n  api_key_in: [header, query]\n  oauth2_flows: []\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: query\n  key: api_key\n  description: |\n    Copado APIs (Actions API, Webhooks API) are authenticated with a Copado API key.\n    Users generate/reset the key from the Copado Account Summary > API Key tab; the key\n    is passed as a parameter on webhook/action callout URLs. Copado Essentials issues a\n    per-account API token used the same way.\n  docs: https://docs.essentials.copado.com/en/articles/6808604-copado-essentials-api-token\nnotes: |\n  Grounded in Copado developer docs, not an OpenAPI securityScheme (Copado publishes its\n  API reference as API Blueprint on Apiary rather than OpenAPI). No OAuth2 scope surface\n  is\
  \ documented for the public developer APIs, so scopes/ is intentionally omitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/copado/refs/heads/main/authentication/copado-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Devops
- Salesforce
- CI/CD
- Release Management
- Testing
- DevSecOps
- Low-Code
---
