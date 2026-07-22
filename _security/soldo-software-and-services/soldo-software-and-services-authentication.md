---
api_key_in: []
api_specs:
- filename: soldo-software-and-services-business-api-openapi.json
  format: json
  label: Soldo Business API
  slug: soldo-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soldo-software-and-services/refs/heads/main/openapi/soldo-software-and-services-business-api-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Soldo Software And Services Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Soldo Software and Services secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Soldo Software and Services
provider_slug: soldo-software-and-services
scheme_count: 1
schemes:
- description: This API uses OAuth 2 with the "Client Credentials" grant flow.
  flows:
  - flow: clientCredentials
    scopes: 44
    tokenUrl: https://api.soldo.com/oauth/authorize
  name: standardAuth
  sources:
  - openapi/soldo-software-and-services-business-api-openapi.json
  type: oauth2
slug: soldo-software-and-services-authentication
source_filename: soldo-software-and-services-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/soldo-software-and-services-business-api-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: standardAuth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.soldo.com/oauth/authorize\n    scopes: 44\n  description: This API uses OAuth 2 with the \"Client Credentials\" grant flow.\n  sources:\n  - openapi/soldo-software-and-services-business-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soldo-software-and-services/refs/heads/main/authentication/soldo-software-and-services-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Spend Management
- Expense Management
- Payments
- Business Cards
- Prepaid Cards
- Fintech
- Financial Services
- Webhooks
---
