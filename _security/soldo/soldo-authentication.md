---
api_key_in: []
api_specs:
- filename: soldo-business-api-v20-openapi-original.json
  format: json
  label: Soldo Business API v2.0
  slug: soldo-business-api-v20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soldo/refs/heads/main/openapi/soldo-business-api-v20-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Soldo Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Soldo secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Soldo
provider_slug: soldo
scheme_count: 1
schemes:
- description: This API uses OAuth 2 with the "Client Credentials" grant flow.
  flows:
  - flow: clientCredentials
    scopes: 44
    tokenUrl: https://api.soldo.com/oauth/authorize
  name: standardAuth
  sources:
  - openapi/soldo-business-api-v20-openapi-original.json
  type: oauth2
slug: soldo-authentication
source_filename: soldo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/soldo-business-api-v20-openapi-original.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: standardAuth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.soldo.com/oauth/authorize\n    scopes: 44\n  description: This API uses OAuth 2 with the \"Client Credentials\" grant flow.\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soldo/refs/heads/main/authentication/soldo-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Consumer
- Fintech
- Financial Services
- Spend Management
- Expense Management
- Business Cards
- Prepaid Cards
- Payments
- Banking
---
