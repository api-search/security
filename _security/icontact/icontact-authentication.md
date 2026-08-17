---
api_key_in: []
api_specs:
- filename: icontact-webhooks-asyncapi.yml
  format: yaml
  label: iContact REST API
  slug: rest-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/icontact/refs/heads/main/asyncapi/icontact-webhooks-asyncapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Icontact Authentication
name_suffix: Authentication
oauth_flows: []
overview: iContact declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: iContact
provider_slug: icontact
scheme_count: 1
schemes:
- headers:
  - description: Uniquely identifies the registered API application. Issued when the integration is created under Settings and Billing > iContact Integrations > Custom API Integrations. A third-party application distributes its own API-AppId, which the account owner must enable at https://app.icontact.com/icp/core/externallogin before use.
    name: API-AppId
    required: true
  - description: The iContact account username used to log in to iContact.
    name: API-Username
    required: true
  - description: The API application password set when the application was registered. The docs state explicitly that this is NOT the iContact login password, and recommend it differ from the account password.
    name: API-Password
    required: true
  - description: Selects the API contract version. Documented accepted values are 2.0, 2.1 and 2.2. The first-party PHP libraries default to 2.2.
    name: API-Version
    required: true
    values:
    - '2.0'
    - '2.1'
    - '2.2'
  id: api-app-headers
  in: header
  rotation: Not documented. The docs describe setting the application password at registration time and say nothing about rotation, expiry or revocation.
  scopes: null
  scopes_note: No scope or permission scoping exists on the credential itself. Authorization is account-level; see the permissions resource (https://help.icontact.com/customers/s/article/Permissions-iContact-API), which grants a USER read/write access per client folder — it does not constrain an API application.
  style: custom-multi-header
  type: apiKey
slug: icontact-authentication
source_filename: icontact-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://help.icontact.com/customers/s/article/API-Getting-Started-Guide\ndocs: https://help.icontact.com/customers/s/article/API-Getting-Started-Guide\nname: iContact REST API authentication\napi: icontact:rest-api\nbase_url: https://app.icontact.com/icp\nsummary: >-\n  iContact authenticates every request with three custom HTTP request headers\n  issued per registered application, not with OAuth, Basic auth or a bearer\n  token. There is no authorization server, no token exchange, no scopes and no\n  refresh; the same three long-lived header values are sent on every call. A\n  fourth header, API-Version, selects the API contract version and is also\n  required.\ntransport:\n  https_required: true\n  https_note: >-\n    The Getting Started guide states \"Every request must be sent over HTTPS.\"\n    Probed 2026-08-13: https://app.icontact.com/icp/time returns\n    strict-transport-security: max-age=15552000; includeSubDomains.\n\
  schemes:\n  - id: api-app-headers\n    type: apiKey\n    in: header\n    style: custom-multi-header\n    headers:\n      - name: API-AppId\n        required: true\n        description: >-\n          Uniquely identifies the registered API application. Issued when the\n          integration is created under Settings and Billing > iContact\n          Integrations > Custom API Integrations. A third-party application\n          distributes its own API-AppId, which the account owner must enable at\n          https://app.icontact.com/icp/core/externallogin before use.\n      - name: API-Username\n        required: true\n        description: The iContact account username used to log in to iContact.\n      - name: API-Password\n        required: true\n        description: >-\n          The API application password set when the application was registered.\n          The docs state explicitly that this is NOT the iContact login\n          password, and recommend it differ from the account password.\n\
  \      - name: API-Version\n        required: true\n        description: >-\n          Selects the API contract version. Documented accepted values are\n          2.0, 2.1 and 2.2. The first-party PHP libraries default to 2.2.\n        values: ['2.0', '2.1', '2.2']\n    rotation: >-\n      Not documented. The docs describe setting the application password at\n      registration time and say nothing about rotation, expiry or revocation.\n    scopes: null\n    scopes_note: >-\n      No scope or permission scoping exists on the credential itself.\n      Authorization is account-level; see the permissions resource\n      (https://help.icontact.com/customers/s/article/Permissions-iContact-API),\n      which grants a USER read/write access per client folder — it does not\n      constrain an API application.\ncontent_negotiation:\n  headers: [Accept, Content-Type]\n  values: [application/json, text/xml]\n  note: >-\n    The API returns 406 Not Acceptable for any other requested representation\n\
  \    and 415 Unsupported Media Type for any other request body format.\nunauthenticated_surface:\n  - path: /icp/time\n    method: GET\n    description: >-\n      The time resource is documented as publicly accessible and is the only\n      documented exception to \"every request must be authenticated\".\n    probed: '2026-08-13'\n    url: https://app.icontact.com/icp/time\n    http_status: 200\n    response: '{\"time\":\"2026-08-13T13:30:19-04:00\",\"timestamp\":1786642219}'\nfailure_behavior:\n  status: 401\n  body: '{\"errors\":[\"Api username invalid\"]}'\n  probed: '2026-08-13'\n  probed_url: https://app.icontact.com/icp/a/\n  note: >-\n    Probed anonymously and with placeholder credentials; both return HTTP 401\n    with the same custom error envelope. No WWW-Authenticate header is sent.\naccount_scoping:\n  required_path_ids: [accountId, clientFolderId]\n  note: >-\n    Almost every resource URI is namespaced /a/{accountId}/c/{clientFolderId}/…\n    Both identifiers are read from\
  \ the iContact UI (Settings and Billing >\n    iContact Integrations > View Details > Account Information), or discovered\n    at runtime by calling GET /a/ then GET /a/{accountId}/c/.\nnot_supported:\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  bearer_token: false\n  hmac_request_signing: false\ngaps:\n  - No OAuth 2.0 or OpenID Connect, so no delegated third-party authorization.\n  - No scopes; a credential that can read contacts can also delete them.\n  - No documented credential rotation, expiry or revocation procedure.\n  - Credentials travel as three separate custom headers on every request.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icontact/refs/heads/main/authentication/icontact-authentication.yml
summary_line: 1 scheme
tags:
- Email Marketing
- Marketing Automation
- Campaigns
- Contacts
- Lists
- Segments
- Webhooks
- Email Deliverability
- SMB
---
