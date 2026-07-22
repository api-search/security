---
api_key_in:
- basic-auth-username
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Uthana Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uthana secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Uthana
provider_slug: uthana
scheme_count: 1
schemes:
- applies_to:
  - https://uthana.com/graphql
  - https://uthana.com/motion/* (REST download endpoints)
  description: HTTP Basic auth with the API key as the username and an empty password (curl -u $API_KEY:). The official Python (uthana) and JS/TS (@uthana/client) clients handle authentication when constructed with the key.
  key_source: Generate the API key in account settings at https://uthana.com/app/account (requires an API-enabled plan).
  name: apiKeyBasic
  scheme: basic
  type: http
slug: uthana-authentication
source_filename: uthana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://uthana.com/docs/api/api-key\ndocs: https://uthana.com/docs/api/api-key\nsummary:\n  types: [http]\n  schemes: [basic]\n  api_key_in: [basic-auth-username]\n  oauth2_flows: []\nschemes:\n  - name: apiKeyBasic\n    type: http\n    scheme: basic\n    description: HTTP Basic auth with the API key as the username and an empty password\n      (curl -u $API_KEY:). The official Python (uthana) and JS/TS (@uthana/client) clients\n      handle authentication when constructed with the key.\n    key_source: Generate the API key in account settings at https://uthana.com/app/account\n      (requires an API-enabled plan).\n    applies_to:\n      - https://uthana.com/graphql\n      - https://uthana.com/motion/* (REST download endpoints)\nnotes:\n  - No OAuth2 / OIDC surface is published (/.well-known/openid-configuration returns 403;\n    no oauth docs).\n  - Docs security guidance - treat the key like a password, store in a secret\
  \ manager or\n    environment variable, rotate via reset_user_apikey if leaked.\n  - Custom API domains are supported via the client `domain` option for non-default hosts.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uthana/refs/heads/main/authentication/uthana-authentication.yml
summary_line: http · 1 scheme
tags:
- Animation
- 3D Characters
- Generative AI
- Motion Capture
- Gaming
- Robotics
- Foundation Models
- GraphQL
---
