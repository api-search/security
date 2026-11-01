---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Figured Authentication
name_suffix: Authentication
oauth_flows: []
overview: Figured declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Figured
provider_slug: figured
scheme_count: 1
schemes:
- authorizationUrl: https://api.figured.com/oauth/authorize
  flow: authorization_code
  scopes: {}
  tokenUrl: https://api.figured.com/oauth/token
  type: oauth2
slug: figured-authentication
source_filename: figured-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://help.figured.com/en/articles/4957587-connecting-to-the-figured-api-with-postman.md\nschemes:\n  - type: oauth2\n    flow: authorization_code\n    authorizationUrl: https://api.figured.com/oauth/authorize\n    tokenUrl: https://api.figured.com/oauth/token\n    scopes: {}\n"
source_yaml_url: https://artifacts.apis.io/figured/authentication/figured-authentication.yml
summary_line: 1 scheme
tags:
- Finance
- Agriculture
- FarmManagement
- SaaS
- Accounting
---
