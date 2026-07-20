---
api_key_in: []
auth_types:
- oauth2
description: Salesforce B2C Commerce (Demandware) authentication documented from the SCAPI and OCAPI authorization guides. No OpenAPI is captured in this repo yet, so this profile is searched from the docs rather than derived from securitySchemes.
kind: authentication
layout: security
method: searched
name: Demandware Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Demandware secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Demandware
provider_slug: demandware
scheme_count: 2
schemes:
- applies_to: SCAPI Shopper APIs and OCAPI Shopper APIs
  audience: shopper
  client_types:
  - public
  - private
  docs: https://developer.salesforce.com/docs/commerce/commerce-api/guide/slas.html
  flows:
  - authorizationCode
  - clientCredentials
  name: SLAS (Shopper Login and API Access Service)
  notes: Grant type depends on client type (public vs private) and shopper auth method. Most clients request tokens via the getAccessToken endpoint.
  standard: OAuth 2.1
  token: ShopperToken (JWT)
  type: oauth2
- applies_to: SCAPI Admin APIs and OCAPI Data API
  audience: admin
  docs: https://developer.salesforce.com/docs/commerce/commerce-api/guide/authorization-for-admin-apis.html
  flows:
  - clientCredentials
  name: Account Manager (AM)
  notes: Admin APIs are secured with Account Manager. Requires an API client registered in Account Manager; the SLAS Admin API/UI requires the SLAS Organization Administrator role.
  token: JWT access token
  type: oauth2
slug: demandware-authentication
source_filename: demandware-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.salesforce.com/docs/commerce/commerce-api/guide/authorization.html\ndocs: https://developer.salesforce.com/docs/commerce/commerce-api/guide/authorization.html\ndescription: >-\n  Salesforce B2C Commerce (Demandware) authentication documented from the SCAPI\n  and OCAPI authorization guides. No OpenAPI is captured in this repo yet, so this\n  profile is searched from the docs rather than derived from securitySchemes.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode, clientCredentials]\n  token_format: JWT\n  token_placement: Authorization Bearer header\nschemes:\n- name: SLAS (Shopper Login and API Access Service)\n  type: oauth2\n  standard: OAuth 2.1\n  audience: shopper\n  applies_to: SCAPI Shopper APIs and OCAPI Shopper APIs\n  flows: [authorizationCode, clientCredentials]\n  client_types: [public, private]\n  token: ShopperToken (JWT)\n  docs: https://developer.salesforce.com/docs/commerce/commerce-api/guide/slas.html\n\
  \  notes: >-\n    Grant type depends on client type (public vs private) and shopper auth method.\n    Most clients request tokens via the getAccessToken endpoint.\n- name: Account Manager (AM)\n  type: oauth2\n  audience: admin\n  applies_to: SCAPI Admin APIs and OCAPI Data API\n  flows: [clientCredentials]\n  token: JWT access token\n  docs: https://developer.salesforce.com/docs/commerce/commerce-api/guide/authorization-for-admin-apis.html\n  notes: >-\n    Admin APIs are secured with Account Manager. Requires an API client registered\n    in Account Manager; the SLAS Admin API/UI requires the SLAS Organization\n    Administrator role.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demandware/refs/heads/main/authentication/demandware-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Commerce
- E-commerce
- Retail
- Commerce Cloud
- Storefront
- Shopper
- Catalog
- Orders
- SaaS
- Salesforce
---
