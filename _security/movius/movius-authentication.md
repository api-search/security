---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Movius Authentication
name_suffix: Authentication
oauth_flows: []
overview: Movius secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Movius
provider_slug: movius
scheme_count: 1
schemes:
- description: Username and password issued to a Management Portal API user, used as HTTP basic credentials when calling the MultiLine Management REST API.
  name: apiUserBasic
  scheme: basic
  sources:
  - https://help.moviuscorp.com/help/add-api-user
  type: http
slug: movius-authentication
source_filename: movius-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://help.moviuscorp.com/help/add-api-user\ndocs: https://help.moviuscorp.com/help/add-api-user\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  notes: >-\n    The MultiLine Management REST API is enterprise-gated. There is no public\n    OpenAPI specification. Access is authenticated with an API user account\n    created in the Movius Management Portal; the API user receives a username\n    and password by email that is then used to consume the API (HTTP basic\n    authentication). API users are scoped to the external application(s) they\n    are authorized for (e.g. HttpApi generic connector, or the MultiLine for\n    Salesforce app).\nschemes:\n- name: apiUserBasic\n  type: http\n  scheme: basic\n  description: >-\n    Username and password issued to a Management Portal API user, used as HTTP\n    basic credentials when calling the MultiLine Management REST API.\n  sources:\n  - https://help.moviuscorp.com/help/add-api-user\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/movius/refs/heads/main/authentication/movius-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Communications
- Messaging
- Mobile
- Telecom
- Compliance
- Security
- Voice
- SMS
- Enterprise
---
