---
api_key_in: []
api_specs:
- filename: paywithmybank-openapi-original.yml
  format: yaml
  label: Trustly Payments API (PayWithMyBank)
  slug: trustly-payments-api-paywithmybank
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paywithmybank/refs/heads/main/openapi/paywithmybank-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Paywithmybank Authentication
name_suffix: Authentication
oauth_flows: []
overview: PayWithMyBank (Trustly) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PayWithMyBank (Trustly)
provider_slug: paywithmybank
scheme_count: 1
schemes:
- credentials: accessId (username) + accessKey (password), provisioned in the Trustly Merchant Portal (Settings > Developer Settings)
  name: HTTPBasic
  scheme: basic
  sources:
  - openapi/paywithmybank-openapi-original.yml
  transport: HTTPS only
  type: http
slug: paywithmybank-authentication
source_filename: paywithmybank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/paywithmybank-openapi-original.yml\ndocs: https://amer.developers.trustly.com/api-reference/api\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\nschemes:\n- name: HTTPBasic\n  type: http\n  scheme: basic\n  credentials: accessId (username) + accessKey (password), provisioned in the Trustly Merchant Portal (Settings > Developer Settings)\n  transport: HTTPS only\n  sources:\n  - openapi/paywithmybank-openapi-original.yml\nnotes:\n- Optional field-level encryption is available for enhanced security.\n- Client-side Lightbox (trustly.js) calls require a server-generated requestSignature in addition to the accessId.\n- No OAuth2/OIDC surface; scopes/ is not applicable for this provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paywithmybank/refs/heads/main/authentication/paywithmybank-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Payments
- Pay by Bank
- Open Banking
- ACH
- Bank Transfers
- Fintech
- Identity Verification
- Webhooks
---
