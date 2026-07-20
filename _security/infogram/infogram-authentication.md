---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Infogram Authentication
name_suffix: Authentication
oauth_flows: []
overview: Infogram secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Infogram
provider_slug: infogram
scheme_count: 1
schemes:
- description: 'API requests authenticate with a personal API token created in the user''s Infogram account settings, passed as an "Authorization: Bearer <token>" header on every request. Tokens inherit the permissions of the account that generated them.'
  format: Bearer <token>
  header: Authorization
  location: header
  name: bearerAuth
  scheme: bearer
  sources:
  - https://api.infogram.com/
  token_source: Infogram account settings
  type: http
slug: infogram-authentication
source_filename: infogram-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.infogram.com/\ndocs: https://api.infogram.com/\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    API requests authenticate with a personal API token created in the user's\n    Infogram account settings, passed as an \"Authorization: Bearer <token>\"\n    header on every request. Tokens inherit the permissions of the account that\n    generated them.\n  location: header\n  header: Authorization\n  format: Bearer <token>\n  token_source: Infogram account settings\n  sources:\n  - https://api.infogram.com/\nnotes: >-\n  No OAuth2/OpenID Connect flows are documented for the current API — access is\n  personal bearer tokens only, so no OAuth scopes artifact applies. The legacy\n  infogr.am API used an API key + shared-secret HMAC signature model; the client\n  libraries in packages/ target\
  \ that legacy scheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infogram/refs/heads/main/authentication/infogram-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Data Visualization
- Infographics
- Charts
- Dashboards
- Reporting
- Business Intelligence
- Content
- Embeds
---
