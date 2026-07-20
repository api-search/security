---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Cato Networks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cato Networks secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cato Networks
provider_slug: cato-networks
scheme_count: 1
schemes:
- description: Cato API key (token) generated in the Cato Management Application (CMA) under API management. Every GraphQL request must include the key in the x-api-key header along with an accountID argument identifying the target account.
  in: header
  name: apiKey
  parameter_name: x-api-key
  sources:
  - https://api.catonetworks.com/documentation/
  type: apiKey
slug: cato-networks-authentication
source_filename: cato-networks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://api.catonetworks.com/documentation/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  description: Cato API key (token) generated in the Cato Management Application (CMA)\n    under API management. Every GraphQL request must include the key in the x-api-key\n    header along with an accountID argument identifying the target account.\n  sources:\n  - https://api.catonetworks.com/documentation/\ndocs: https://api.catonetworks.com/documentation/\naccount_scope: Requests are bound to a Cato account via an accountID variable; the\n  API key is generated per account/admin and can be scoped by admin role and API\n  permissions in the CMA.\nnotes: No OAuth 2.0 / OpenID Connect surface. Authentication is a single API key\n  header (x-api-key); there is no scopes artifact because the API does not expose\n  OAuth\
  \ scopes (permissions are governed by CMA admin roles).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cato-networks/refs/heads/main/authentication/cato-networks-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cybersecurity
- SASE
- SSE
- Networking
- Security
- SD-WAN
- Zero Trust
- GraphQL
- API
---
