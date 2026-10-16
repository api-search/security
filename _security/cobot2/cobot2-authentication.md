---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cobot2-openapi.yml
  format: yaml
  label: Cobot API
  slug: cobot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cobot2/refs/heads/main/openapi/cobot2-openapi.yml
auth_types: []
description: Cobot uses OAuth2 for API authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cobot2 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cobot2 declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Cobot2
provider_slug: cobot2
scheme_count: 1
schemes:
- authorize_url: https://www.cobot.me/oauth/authorize
  evidence: This is a step-by-step guide on authenticating against our API.
  flows:
  - authorization_code
  - password
  how_to_obtain: Register an app to receive a client id and secret, then follow the OAuth2 web flow or the app flow to obtain an access token.
  name: OAuth2
  type: oauth2
slug: cobot2-authentication
source_filename: cobot2-authentication.yml
source_heading: Authentication Profile
source_url: https://www.cobot.me/login
source_yaml: "generated: '2026-10-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.cobot.me/login\nsources:\n- https://www.cobot.me/login\n- https://dev.cobot.me/page/oauth-flow\n- https://www.cobot.me/login\ndescription: Cobot uses OAuth2 for API authentication.\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: This is a step-by-step guide on authenticating against our API.\n  flows:\n  - authorization_code\n  - password\n  authorize_url: https://www.cobot.me/oauth/authorize\n  how_to_obtain: Register an app to receive a client id and secret, then follow the OAuth2 web flow or the app flow to obtain an access token.\nnote: 'Access tokens can be sent as a query parameter called access_token or as an HTTP header \"Authorization: Bearer <token>\".'\ndocs: https://www.cobot.me/login\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cobot2/refs/heads/main/authentication/cobot2-authentication.yml
summary_line: 1 scheme
tags:
- Coworking
- SaaS
- Management
- Software
- Collaboration
- Company
---
