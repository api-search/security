---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Cross River Bank Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cross River Bank secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cross River Bank
provider_slug: cross-river-bank
scheme_count: 1
schemes:
- description: 'OAuth 2.0 client credentials grant. Partners are provisioned a client_id and client_secret during onboarding, then POST client_id, client_secret, and grant_type=client_credentials (optionally audience and scope) to the COS identity provider token endpoint. The sandbox token endpoint is https://idptest.crbcos.com/connect/token; the lending module uses https://oauthtest.crbnj.net/connect/token. The response is a signed JWT that must be sent as `Authorization: Bearer <token>` on every API request.'
  flow: clientCredentials
  name: oauth2ClientCredentials
  sources:
  - https://docs.crossriver.com/get-started/quickstart/get-access-token
  - https://docs.crossriver.com/get-started/api-basics
  - openapi/cross-river-openapi.yml
  tokenUrl: https://idptest.crbcos.com/connect/token
  type: oauth2
slug: cross-river-bank-authentication
source_filename: cross-river-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: docs.crossriver.com + openapi/cross-river-openapi.yml\nsummary:\n  types:\n  - oauth2\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://idptest.crbcos.com/connect/token\n  description: >-\n    OAuth 2.0 client credentials grant. Partners are provisioned a client_id and\n    client_secret during onboarding, then POST client_id, client_secret, and\n    grant_type=client_credentials (optionally audience and scope) to the COS\n    identity provider token endpoint. The sandbox token endpoint is\n    https://idptest.crbcos.com/connect/token; the lending module uses\n    https://oauthtest.crbnj.net/connect/token. The response is a signed JWT that\n    must be sent as `Authorization: Bearer <token>` on every API request.\n  sources:\n  - https://docs.crossriver.com/get-started/quickstart/get-access-token\n  - https://docs.crossriver.com/get-started/api-basics\n  - openapi/cross-river-openapi.yml\n\
  notes: >-\n  Access is partner/enterprise-gated - there is no open self-service signup.\n  Credentials for sandbox and, later, production are issued by Cross River during\n  onboarding. Production token/host URLs are provisioned at go-live and are not\n  published in the open documentation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cross-river-bank/refs/heads/main/authentication/cross-river-bank-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Banking
- Banking as a Service
- Sponsor Bank
- Embedded Finance
- Payments
- ACH
- RTP
- FedNow
- Cards
- Lending
- Stablecoins
---
