---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Favro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Favro secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Favro
provider_slug: favro
scheme_count: 1
schemes:
- credential: email + API token
  description: HTTP Basic authentication. The username is the account email address; the password is either the account password or, recommended, a per-user API token generated from the Favro user profile. API tokens are revocable at any time and can be restricted to read-only endpoints.
  name: basicAuth
  read_only_tokens: true
  revocable: true
  scheme: basic
  sources:
  - docs
  token_management: https://favro.com/organization/ (user profile > API tokens)
  type: http
slug: favro-authentication
source_filename: favro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://favro.com/developer\ndocs: https://favro.com/developer\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication. The username is the account email address; the\n    password is either the account password or, recommended, a per-user API\n    token generated from the Favro user profile. API tokens are revocable at\n    any time and can be restricted to read-only endpoints.\n  credential: email + API token\n  token_management: https://favro.com/organization/ (user profile > API tokens)\n  read_only_tokens: true\n  revocable: true\n  sources: [docs]\nnotes:\n- Organization-scoped requests additionally require an organizationId header.\n- No OAuth 2.0 / OpenID Connect authorization surface is documented; the API\n  is key/token based via HTTP Basic.\n- SCIM 1.1 and 2.0 provisioning\
  \ endpoints use bearer-token authentication\n  configured per Favro organization.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/favro/refs/heads/main/authentication/favro-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Saas
- Project Management
- Collaboration
- Agile
- Planning
- Task Management
- Kanban
- Productivity
---
