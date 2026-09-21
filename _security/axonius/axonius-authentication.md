---
anonymous_access: false
api_key_in: []
api_specs:
- filename: postman-minis
  format: yaml
  label: Axonius
  slug: axonius
  spec_type: Postman
  url: https://github.com/Axonius/postman-minis
auth_types:
- apiKey
- oauth2
description: 'Authentication profile for the Axonius REST API, read from the public docs (no OpenAPI is published outside the login-gated developer.axonius.com reference). The API is reachable only through a dedicated SERVICE ACCOUNT (Axonius v6.1.74 and later; regular user accounts worked through v6.1.73) whose role grants API access and the permissions it needs. A service account authenticates one of two ways: an API key + API secret pair sent as request headers (the default, and the scheme the provider''s own Postman collections and Python client use), or OAuth 2.1 client credentials exchanged at the instance''s /api/oauth2/token endpoint for a one-hour bearer token. The instance host is customer-specific ({axonius-instance}).'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Axonius Authentication
name_suffix: Authentication
oauth_flows: []
overview: Axonius secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Axonius
provider_slug: axonius
scheme_count: 2
schemes:
- description: Default scheme. The system generates an API key and secret pair when the service account is saved; both are included in each API request as the api-key and api-secret headers. The secret is displayed once and cannot be recovered — reset the key to get a new secret.
  evidence:
  - https://docs.axonius.com/docs/manage-service-accounts
  - https://github.com/Axonius/postman-minis (api-key / api-secret headers on every request)
  headers:
  - api-key
  - api-secret
  in: header
  name: apiKeyAndSecret
  type: apiKey
- description: OAuth 2.1 option on a service account. Client ID and Client Secret are exchanged for a short-lived access token (expires after one hour); permissions come from the service account's role and data scope, not from OAuth scopes — no scope list is published.
  evidence:
  - https://docs.axonius.com/docs/manage-service-accounts#using-oauth-21-authentication
  flows:
    clientCredentials:
      scopes: {}
      tokenUrl: https://{axonius-instance}/api/oauth2/token
  name: oauth21ClientCredentials
  reset_endpoint: POST /api/settings/service_accounts/<service_account_id>/reset_credentials
  scopes_documented: false
  token_lifetime: 1 hour
  token_request:
    auth: HTTP Basic — base64(client_id:client_secret)
    body: application/x-www-form-urlencoded, grant_type=client_credentials
    method: POST
  type: oauth2
  usage: Authorization Bearer <access_token> on each API request
slug: axonius-authentication
source_filename: axonius-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: searched\nsource: https://docs.axonius.com/docs/manage-service-accounts\ndocs: https://docs.axonius.com/docs/axonius-rest-api\ndescription: >-\n  Authentication profile for the Axonius REST API, read from the public docs (no OpenAPI is\n  published outside the login-gated developer.axonius.com reference). The API is reachable only\n  through a dedicated SERVICE ACCOUNT (Axonius v6.1.74 and later; regular user accounts worked\n  through v6.1.73) whose role grants API access and the permissions it needs. A service account\n  authenticates one of two ways: an API key + API secret pair sent as request headers (the\n  default, and the scheme the provider's own Postman collections and Python client use), or\n  OAuth 2.1 client credentials exchanged at the instance's /api/oauth2/token endpoint for a\n  one-hour bearer token. The instance host is customer-specific ({axonius-instance}).\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  service_account_required:\
  \ true\n  key_secret_shown_once: true\n  rotation: API key can be rotated at any time; resetting OAuth credentials invalidates all existing access tokens for that service account\nschemes:\n- name: apiKeyAndSecret\n  type: apiKey\n  in: header\n  headers:\n  - api-key\n  - api-secret\n  description: >-\n    Default scheme. The system generates an API key and secret pair when the service account is\n    saved; both are included in each API request as the api-key and api-secret headers. The\n    secret is displayed once and cannot be recovered — reset the key to get a new secret.\n  evidence:\n  - https://docs.axonius.com/docs/manage-service-accounts\n  - https://github.com/Axonius/postman-minis (api-key / api-secret headers on every request)\n- name: oauth21ClientCredentials\n  type: oauth2\n  flows:\n    clientCredentials:\n      tokenUrl: https://{axonius-instance}/api/oauth2/token\n      scopes: {}\n  token_request:\n    method: POST\n    auth: HTTP Basic — base64(client_id:client_secret)\n\
  \    body: application/x-www-form-urlencoded, grant_type=client_credentials\n  token_lifetime: 1 hour\n  usage: Authorization Bearer <access_token> on each API request\n  reset_endpoint: POST /api/settings/service_accounts/<service_account_id>/reset_credentials\n  scopes_documented: false\n  description: >-\n    OAuth 2.1 option on a service account. Client ID and Client Secret are exchanged for a\n    short-lived access token (expires after one hour); permissions come from the service\n    account's role and data scope, not from OAuth scopes — no scope list is published.\n  evidence:\n  - https://docs.axonius.com/docs/manage-service-accounts#using-oauth-21-authentication\nnotes:\n- Advanced API settings toggle enables the /users/destroy and /devices/destroy endpoints and cross-domain calls from the developer.axonius.com reference (https://docs.axonius.com/docs/managing-api-settings).\n- The deprecated axonius_api_client reads AX_URL, AX_KEY and AX_SECRET from the environment.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axonius/refs/heads/main/authentication/axonius-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Asset Management
- Cybersecurity
- SaaS Management
- SaaS Security
- Vulnerability Management
- IT Asset Management
- Security Operations
---
