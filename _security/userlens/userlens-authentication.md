---
api_key_in: []
api_specs:
- filename: userlens-events-openapi.yml
  format: yaml
  label: Userlens Events API
  slug: userlens-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/userlens/refs/heads/main/openapi/userlens-events-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Userlens Authentication
name_suffix: Authentication
oauth_flows: []
overview: Userlens secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Userlens
provider_slug: userlens
scheme_count: 1
schemes:
- credential:
    name: Write Code
    obtain_from: https://app.userlens.io/settings/integrations/userlens-sdk
  description: All API requests require the account Write Code in the Authorization header using HTTP Basic Auth. The token is the base64 encoding of "write_code:" (write code as username, trailing colon, empty password). The Write Code is issued in the Userlens app at Settings > Integrations > Userlens SDK.
  name: writeCodeBasicAuth
  scheme: basic
  sources:
  - openapi/userlens-events-openapi.yml
  type: http
slug: userlens-authentication
source_filename: userlens-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://userlens.gitbook.io/userlens-analytics/guides/api-reference\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  oauth2_flows: []\nschemes:\n  - name: writeCodeBasicAuth\n    type: http\n    scheme: basic\n    description: All API requests require the account Write Code in the Authorization\n      header using HTTP Basic Auth. The token is the base64 encoding of \"write_code:\"\n      (write code as username, trailing colon, empty password). The Write Code is\n      issued in the Userlens app at Settings > Integrations > Userlens SDK.\n    credential:\n      name: Write Code\n      obtain_from: https://app.userlens.io/settings/integrations/userlens-sdk\n    sources: [openapi/userlens-events-openapi.yml]\nnotes:\n  - No OAuth 2.0, OpenID Connect, or API-key-in-query schemes are documented for\n    the Events API.\n  - The product app advertises OKTA/SSO access on the Enterprise plan (pricing\n    page), which applies\
  \ to dashboard login, not the Events API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/userlens/refs/heads/main/authentication/userlens-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Customer Success
- Product Analytics
- AI Agents
- Churn Prediction
- Event Tracking
- B2B SaaS
- Account Intelligence
---
