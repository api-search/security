---
api_key_in: []
api_specs:
- filename: zettle-finance-api-openapi.yaml
  format: yaml
  label: Zettle Finance API
  slug: zettle-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zettle/refs/heads/main/openapi/zettle-finance-api-openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zettle Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Zettle secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Zettle
provider_slug: zettle
scheme_count: 1
schemes:
- description: For more information, see the [OAuth API documentation](https://developer.zettle.com/docs/api/oauth/overview).
  flows:
  - authorizationUrl: https://oauth.zettle.com/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://oauth.zettle.com/token
  name: ZettleOauth
  sources:
  - openapi/zettle-finance-api-openapi.yaml
  type: oauth2
slug: zettle-authentication
source_filename: zettle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zettle-finance-api-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ZettleOauth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.zettle.com/authorize\n    tokenUrl: https://oauth.zettle.com/token\n    scopes: 1\n  description: For more information, see the [OAuth API documentation](https://developer.zettle.com/docs/api/oauth/overview).\n  sources:\n  - openapi/zettle-finance-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zettle/refs/heads/main/authentication/zettle-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Point of Sale
- POS
- Payments
- Inventory
- Finance
- PayPal
- Card Payments
- Merchant Services
---
