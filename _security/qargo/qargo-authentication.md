---
api_key_in: []
api_specs:
- filename: qargo-tms-openapi-original.yml
  format: yaml
  label: Qargo TMS API
  slug: qargo-tms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qargo/refs/heads/main/openapi/qargo-tms-openapi-original.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Qargo Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Qargo secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Qargo
provider_slug: qargo
scheme_count: 2
schemes:
- applies_to: REST API
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.qargo.com/v1/auth/token
    token_format: JWT
  name: oAuth2ClientCredentials
  sources:
  - openapi/qargo-tms-openapi-original.yml
  type: oauth2
- applies_to: Webhooks
  name: BasicAuthWebhookCredentials
  provisioned_by: Qargo (integrations@qargo.com)
  scheme: basic
  sources:
  - openapi/qargo-tms-openapi-original.yml
  type: http
slug: qargo-authentication
source_filename: qargo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/qargo-tms-openapi-original.yml\ndocs: https://api-docs.qargo.com/docs/section/authentication/the-api-call-to-request-tokens\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - clientCredentials\n  note: >-\n    The Qargo TMS REST API uses OAuth2 client-credentials (service-to-service). A JWT\n    access token is obtained from POST https://api.qargo.com/v1/auth/token using HTTP\n    Basic auth (client_id:secret_id, base64) and refreshed on expiry (expires_in).\n    Application clients are created by a Super admin under Configuration -> Organisation\n    Settings and must be linked to an approved integration id. Webhooks use a SEPARATE\n    HTTP Basic scheme (BasicAuthWebhookCredentials), provisioned by Qargo — OAuth tokens\n    must not be used for webhooks.\nschemes:\n- name: oAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.qargo.com/v1/auth/token\n\
  \    token_format: JWT\n    scopes: 0\n  applies_to: REST API\n  sources:\n  - openapi/qargo-tms-openapi-original.yml\n- name: BasicAuthWebhookCredentials\n  type: http\n  scheme: basic\n  applies_to: Webhooks\n  provisioned_by: Qargo (integrations@qargo.com)\n  sources:\n  - openapi/qargo-tms-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qargo/refs/heads/main/authentication/qargo-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Transport Management
- Logistics
- Supply Chain
- Freight
- TMS
- Accounting
- Webhooks
---
