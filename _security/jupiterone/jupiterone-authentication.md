---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Jupiterone Authentication
name_suffix: Authentication
oauth_flows: []
overview: JupiterOne secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: JupiterOne
provider_slug: jupiterone
scheme_count: 2
schemes:
- applies_to: https://graphql.us.jupiterone.io/ and https://api.us.jupiterone.io/
  description: 'Every request sends Authorization: Bearer <API_KEY>. The token is a JupiterOne API key created in the account. Wildcards are not supported in tokens.'
  name: bearerAuth
  scheme: bearer
  type: http
- description: The JupiterOne account id must accompany every request. Found under Settings > Account Management (apps.us.jupiterone.io/settings/account-management).
  in: header
  name: accountHeader
  parameter: JupiterOne-Account
  type: apiKey
slug: jupiterone-authentication
source_filename: jupiterone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.jupiterone.io/api/authentication\ndocs: https://docs.jupiterone.io/api/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  oauth2: false\n  additional_required_headers:\n  - JupiterOne-Account\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Every request sends Authorization: Bearer <API_KEY>. The token is a JupiterOne\n    API key created in the account. Wildcards are not supported in tokens.\n  applies_to: https://graphql.us.jupiterone.io/ and https://api.us.jupiterone.io/\n- name: accountHeader\n  type: apiKey\n  in: header\n  parameter: JupiterOne-Account\n  description: >-\n    The JupiterOne account id must accompany every request. Found under Settings >\n    Account Management (apps.us.jupiterone.io/settings/account-management).\nkey_types:\n- name: Account-level API key\n  description: >-\n    Created via the CreateToken GraphQL mutation or the\
  \ dashboard (Settings >\n    Account Management, Administrator permission required). Governed by a JSON\n    permission policy with effect (ALLOW/DENY), actions, and resources; conditions\n    such as stringEquals can constrain query:ReadGraphData.\n- name: Integration API key\n  description: >-\n    Scoped to synchronizing data within a single integration; cannot read the graph\n    or perform other system actions.\nregions:\n  us:\n    graphql: https://graphql.us.jupiterone.io\n    rest: https://api.us.jupiterone.io\n  eu:\n    graphql: https://graphql.eu.jupiterone.io\n    rest: https://api.eu.jupiterone.io\nnotes: >-\n  No OAuth 2.0 or OpenID Connect flow is documented; authentication is Bearer API\n  key plus the JupiterOne-Account header. Permission policies provide fine-grained,\n  resource/action-scoped authorization rather than OAuth scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jupiterone/refs/heads/main/authentication/jupiterone-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Security
- CAASM
- Cyber Asset Management
- Attack Surface Management
- Cloud Security
- Graph
- GraphQL
- Compliance
- Asset Intelligence
---
