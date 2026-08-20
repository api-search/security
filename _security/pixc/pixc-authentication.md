---
api_key_in: []
api_specs:
- filename: schema
  format: yaml
  label: Pixc Public API
  slug: pixc-public-api
  spec_type: OpenAPI
  url: https://dashboard.pixc.com/v1/schema
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Pixc Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Pixc secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Pixc
provider_slug: pixc
scheme_count: 2
schemes:
- description: OAuth 2.0 implicit flow declared in securityDefinitions.pixc_auth of the Pixc-published Swagger 2.0 document. Applied with a scoped requirement on every operation (see scopes/pixc-scopes.yml for the full eleven-scope list).
  flows:
  - authorizationUrl: https://dashboard.pixc.com/v1/oauth
    flow: implicit
    refreshUrl: null
    scopes: 11
    tokenUrl: null
  method: derived
  name: pixc_auth
  sources:
  - openapi/pixc-orders-api-openapi.yml
  - openapi/pixc-templates-api-openapi.yml
  - openapi/pixc-webhooks-api-openapi.yml
  type: oauth2
- description: 'Long-lived personal Access Token obtained from Account Settings > API Access in the Pixc Dashboard. This is the mechanism the Getting Started docs demonstrate, verbatim: "First of all, you need an Access Token. It can be obtained under Account Settings > API Access section of Pixc Dashboard." The first-party Node SDK takes the same value as its required `token` option.'
  format: Bearer ACCESS_TOKEN
  header: Authorization
  in: header
  method: searched
  name: access_token
  scheme: bearer
  sources:
  - https://pixc.com/api/
  - https://github.com/Pixc2/pixc-api-node
  type: http
slug: pixc-authentication
source_filename: pixc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/pixc-orders-api-openapi.yml, openapi/pixc-templates-api-openapi.yml, openapi/pixc-webhooks-api-openapi.yml\ndocs: https://pixc.com/api/\ntoken_page: https://pixc.com/dashboard/account/api\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - implicit\n  http_schemes:\n  - bearer\n  note: >-\n    The published Swagger declares exactly one security scheme — an OAuth 2.0 implicit flow\n    with eleven scopes — and applies it to all sixteen operations. But the provider's own\n    Getting Started documentation does not use that flow: it instructs developers to copy a\n    long-lived personal Access Token out of the dashboard and send it as\n    `Authorization: Bearer ACCESS_TOKEN`. The bearer entry below is therefore recorded from\n    the docs, not from the spec, and is the path a developer actually takes.\nschemes:\n- name: pixc_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://dashboard.pixc.com/v1/oauth\n\
  \    tokenUrl: null\n    refreshUrl: null\n    scopes: 11\n  description: >-\n    OAuth 2.0 implicit flow declared in securityDefinitions.pixc_auth of the\n    Pixc-published Swagger 2.0 document. Applied with a scoped requirement on every\n    operation (see scopes/pixc-scopes.yml for the full eleven-scope list).\n  method: derived\n  sources:\n  - openapi/pixc-orders-api-openapi.yml\n  - openapi/pixc-templates-api-openapi.yml\n  - openapi/pixc-webhooks-api-openapi.yml\n- name: access_token\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer ACCESS_TOKEN'\n  description: >-\n    Long-lived personal Access Token obtained from Account Settings > API Access in the Pixc\n    Dashboard. This is the mechanism the Getting Started docs demonstrate, verbatim:\n    \"First of all, you need an Access Token. It can be obtained under Account Settings >\n    API Access section of Pixc Dashboard.\" The first-party Node SDK takes the same value as\n    its required\
  \ `token` option.\n  method: searched\n  sources:\n  - https://pixc.com/api/\n  - https://github.com/Pixc2/pixc-api-node\n\nobserved_behavior:\n  probe: GET https://dashboard.pixc.com/v1/api/order\n  checked: '2026-08-13'\n  no_credential: {status: 403, body: '{\"message\":\"API Error\",\"success\":false}'}\n  invalid_bearer: {status: 403, body: '{\"message\":\"API Error\",\"success\":false}'}\n  note: >-\n    Byte-identical responses with no `code` field, and 403 is not declared anywhere in the\n    published spec (which declares only 200 and 400). A client cannot distinguish a missing\n    credential from an invalid one from insufficient scope.\n\nweaknesses:\n- >-\n  The declared OAuth 2.0 grant is the implicit flow, which RFC 9700 (OAuth 2.0 Security Best\n  Current Practice) says must no longer be used. No authorization-code flow, no PKCE, no\n  tokenUrl and no refreshUrl are declared.\n- >-\n  No token lifetime, rotation or revocation procedure is documented for the personal Access\n\
  \  Token, and no /.well-known/oauth-authorization-server metadata is served (404).\n- The authentication failure status is undocumented and carries no machine-readable code.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixc/refs/heads/main/authentication/pixc-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Shopify
- E-Commerce
- Photo Editing
- Image Optimization
- Image Processing
- Product Photography
- Background Removal
- SEO
- Automation
- Artificial Intelligence
- Webhook
- Digital Asset Management
---
