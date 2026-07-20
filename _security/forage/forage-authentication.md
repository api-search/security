---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Forage Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Forage secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Forage
provider_slug: forage
scheme_count: 2
schemes:
- bulk_revoke_endpoint: https://api.joinforage.app/o/bulk_revoke/
  description: Long-lived OAuth 2.0 bearer token created with a POST to /o/token/ using the app's Client ID and Client Secret from the Forage dashboard. Used in the Authorization header of server-side requests for sensitive tasks (create order, capture payment). Default expiry 7 days (604800s), configurable up to 30 days. Up to 1000 active tokens per Client ID/Secret pair; revoke via /o/revoke_token/ or /o/bulk_revoke/.
  expiry_default_seconds: 604800
  flow: clientCredentials
  name: authentication_token
  revoke_endpoint: https://api.joinforage.app/o/revoke_token/
  scope: server-side
  token_endpoint: https://api.joinforage.app/o/token/
  type: oauth2
- description: Short-lived OAuth 2.0 bearer token created with a POST to /session_token/ from a valid authentication token. Expires after 15 minutes. Required for client-side requests and SDK methods that submit customer data (e.g. create PaymentMethod).
  expiry_seconds: 900
  name: session_token
  scheme: bearer
  scope: client-side
  token_endpoint: https://api.joinforage.app/session_token/
  type: http
slug: forage-authentication
source_filename: forage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.joinforage.app/docs/authentication\ndocs: https://docs.joinforage.app/docs/authentication-concepts\nsummary:\n  types: [oauth2, http]\n  scheme: bearer\n  oauth2_flows: [clientCredentials]\n  model: >-\n    OAuth 2.0 bearer tokens. Long-lived authentication tokens are minted from a\n    Client ID + Client Secret for server-side requests; short-lived session tokens\n    are minted from an authentication token for client-side / SDK requests. Tokens\n    are passed in the HTTP Authorization header.\nschemes:\n- name: authentication_token\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    Long-lived OAuth 2.0 bearer token created with a POST to /o/token/ using the\n    app's Client ID and Client Secret from the Forage dashboard. Used in the\n    Authorization header of server-side requests for sensitive tasks (create order,\n    capture payment). Default expiry 7 days (604800s), configurable up to 30\
  \ days.\n    Up to 1000 active tokens per Client ID/Secret pair; revoke via /o/revoke_token/\n    or /o/bulk_revoke/.\n  token_endpoint: https://api.joinforage.app/o/token/\n  revoke_endpoint: https://api.joinforage.app/o/revoke_token/\n  bulk_revoke_endpoint: https://api.joinforage.app/o/bulk_revoke/\n  expiry_default_seconds: 604800\n  scope: server-side\n- name: session_token\n  type: http\n  scheme: bearer\n  description: >-\n    Short-lived OAuth 2.0 bearer token created with a POST to /session_token/ from\n    a valid authentication token. Expires after 15 minutes. Required for client-side\n    requests and SDK methods that submit customer data (e.g. create PaymentMethod).\n  token_endpoint: https://api.joinforage.app/session_token/\n  expiry_seconds: 900\n  scope: client-side\nnotes:\n- The Merchant-Account header is required for HSA/FSA and credit/debit payment methods;\n  optional for EBT payment methods (EBT PaymentMethods are tenant-scoped).\n- Sandbox credentials are managed\
  \ at https://dashboard.sandbox.joinforage.app/ and\n  production at https://dashboard.joinforage.app/.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/authentication/forage-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Payments
- EBT
- SNAP
- EBT Cash
- HSA/FSA
- Fintech
- Government Benefits
- Grocery
- Checkout
- Financial Services
---
