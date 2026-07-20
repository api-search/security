---
api_key_in: []
auth_types:
- session-cookie
description: ''
kind: authentication
layout: security
method: searched
name: Ctera Authentication
name_suffix: Authentication
oauth_flows: []
overview: CTERA secures its APIs with session-cookie across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CTERA
provider_slug: ctera
scheme_count: 1
schemes:
- base_url_pattern: https://<tenant>.ctera.com/admin/api
  failure_status: 403
  login:
    content_type: application/x-www-form-urlencoded
    endpoint: '{BASE_URL}/login'
    method: POST
    on_success: Server sets HTTP session cookies that must be returned on all subsequent requests.
    params:
    - description: Administrator user account name.
      name: j_username
    - description: User password (transmitted over HTTPS).
      name: j_password
  logout:
    body: empty
    endpoint: '{BASE_URL}/logout'
    method: POST
    result: Session terminated (200 OK).
  name: portalSessionLogin
  session:
    note: Same HTTP client (cookie jar) must be reused across requests.
    timeout_minutes: 30
  sources:
  - https://www.ctera.com/help/portal/6.0/api/
  type: session-cookie
slug: ctera-authentication
source_filename: ctera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.ctera.com/help/portal/6.0/api/\ndocs: https://www.ctera.com/help/portal/6.0/api/CTERA%20Portal%20APIs/CTERA_Portal_API_Developer_Guide3.html\nsummary:\n  types: [session-cookie]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The CTERA Portal RESTful API uses form-based login that establishes an HTTP\n    session cookie; there is no OAuth2/OIDC or API-key scheme. The CTERA Python\n    SDK and both MCP servers authenticate with the same administrator\n    username/password credentials.\nschemes:\n  - name: portalSessionLogin\n    type: session-cookie\n    login:\n      endpoint: \"{BASE_URL}/login\"\n      method: POST\n      content_type: application/x-www-form-urlencoded\n      params:\n        - name: j_username\n          description: Administrator user account name.\n        - name: j_password\n          description: User password (transmitted over HTTPS).\n      on_success: Server sets HTTP session cookies\
  \ that must be returned on all subsequent requests.\n    logout:\n      endpoint: \"{BASE_URL}/logout\"\n      method: POST\n      body: empty\n      result: Session terminated (200 OK).\n    session:\n      timeout_minutes: 30\n      note: Same HTTP client (cookie jar) must be reused across requests.\n    base_url_pattern: \"https://<tenant>.ctera.com/admin/api\"\n    failure_status: 403\n    sources:\n      - https://www.ctera.com/help/portal/6.0/api/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ctera/refs/heads/main/authentication/ctera-authentication.yml
summary_line: session-cookie · 1 scheme
tags:
- Company
- Cloud
- Storage
- File Storage
- Global File System
- Data Management
- Edge Computing
- Cyber Protection
- Hybrid Cloud
- Unstructured Data
---
