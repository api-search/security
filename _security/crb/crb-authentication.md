---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Crb Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: CRB secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: CRB
provider_slug: crb
scheme_count: 1
schemes:
- description: Cross River COS API access uses OAuth2 client credentials. Developers register to receive a client id and client secret, exchange them for a bearer access token, and include that token in the Authorization header of each API call. The sandbox is a fully isolated environment with its own credentials.
  flow: clientCredentials
  name: OAuth2ClientCredentials
  sources:
  - https://docs.crossriver.com/get-started/quickstart
  token_delivery: Authorization header (Bearer access token)
  type: oauth2
slug: crb-authentication
source_filename: crb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.crossriver.com/get-started/quickstart\ndocs: https://docs.crossriver.com/get-started/quickstart\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    Cross River COS API access uses OAuth2 client credentials. Developers\n    register to receive a client id and client secret, exchange them for a\n    bearer access token, and include that token in the Authorization header of\n    each API call. The sandbox is a fully isolated environment with its own\n    credentials.\n  token_delivery: Authorization header (Bearer access token)\n  sources:\n  - https://docs.crossriver.com/get-started/quickstart\nnotes: >-\n  Token and authorization endpoint URLs and OAuth scopes are provisioned per\n  partner during onboarding and are not published on the public documentation;\n  no OpenAPI securitySchemes\
  \ were available to derive them.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crb/refs/heads/main/authentication/crb-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Banking
- Banking as a Service
- Embedded Finance
- Payments
- Fintech
- Lending
- Cards
- ACH
- API
---
