---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Appdome Authentication
name_suffix: Authentication
oauth_flows: []
overview: Appdome secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Appdome
provider_slug: appdome
scheme_count: 1
schemes:
- bearer_format: opaque
  description: 'Appdome''s Build2Secure API Token, passed in the Authorization header as a bearer token (Authorization: Bearer <token>). The token is obtained from the Appdome account under the ''Account and API'' section of the User/API menu.'
  header: Authorization
  location: header
  name: build2secureToken
  scheme: bearer
  type: http
slug: appdome-authentication
source_filename: appdome-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://apis.appdome.com/docs/getting-started\ndocs: https://apis.appdome.com/reference/get_upload-link\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: build2secureToken\n  type: http\n  scheme: bearer\n  bearer_format: opaque\n  description: >-\n    Appdome's Build2Secure API Token, passed in the Authorization header as a bearer\n    token (Authorization: Bearer <token>). The token is obtained from the Appdome\n    account under the 'Account and API' section of the User/API menu.\n  location: header\n  header: Authorization\ntoken_management:\n  obtain: https://fusion.appdome.com/ -> User Menu -> Account and API\n  refresh_endpoint: POST https://fusion.appdome.com/api/v1/refreshApiToken\n  company_user_refresh: POST /mycompany/users/{userId}/refreshtoken\nidentity_context:\n  - team_id: required when operating within a team\n  - fusion_set_id: identifies the security\
  \ configuration used to build\nnotes: >-\n  Single bearer-token model (no OAuth2 / OIDC on the public API). SSO options\n  (Azure, Okta, Ping, Passkey) exist for console login and are recorded as DEV-Logs\n  login events, but the REST API authenticates exclusively with the Build2Secure\n  bearer token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appdome/refs/heads/main/authentication/appdome-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Mobile App Security
- Mobile App Defense
- DevSecOps
- Application Security
- Mobile
- CI/CD
- App Signing
- Anti-Fraud
- Code Signing
---
