---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Litmus Automation Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- password
overview: Litmus Automation secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and password flow(s).
provider_name: Litmus Automation
provider_slug: litmus-automation
scheme_count: 2
schemes:
- applies_to:
  - Litmus Edge
  - Litmus Unify
  flows:
  - flow: clientCredentials
    grant: client_credentials
    request: 'POST {{edgeUrl}}/auth/v3/oauth/token, Content-Type: application/x-www-form-urlencoded, body grant_type=client_credentials&client_id=<id>&client_secret=<secret>'
    response: '{"access_token": "...", "expires_in": 3600}'
    tokenUrl: '{{edgeUrl}}/auth/v3/oauth/token'
  - flow: password
    grant: password
    note: Password grant also documented for Litmus Edge / Litmus Unify.
  name: LitmusEdgeOAuth2
  type: oauth2
  usage: 'Send the access_token as Authorization: Bearer <token> on every call. Tokens expire in 3600s; refresh before expiry. Do NOT call the Keycloak-style path.'
- applies_to:
  - Litmus Edge Manager
  in: header
  name: LitmusEdgeManagerAdminToken
  name_header: X-AuthToken
  note: LEM uses an admin API token supplied in the X-AuthToken header. A /auth/validate endpoint validates tokens.
  type: apiKey
slug: litmus-automation-authentication
source_filename: litmus-automation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.litmus.io/le/agents.md\ndocs: https://api.litmus.io/reference/variables.md\nnotes: 'No downloadable OpenAPI spec is published (the API portal serves a proprietary\n  agents.md / llms.txt navigation tree), so this profile is captured from the published\n  API documentation rather than derived from securitySchemes.'\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  oauth2_flows:\n  - clientCredentials\n  - password\n  api_key_in:\n  - header\nschemes:\n- name: LitmusEdgeOAuth2\n  type: oauth2\n  applies_to:\n  - Litmus Edge\n  - Litmus Unify\n  flows:\n  - flow: clientCredentials\n    tokenUrl: '{{edgeUrl}}/auth/v3/oauth/token'\n    grant: client_credentials\n    request: 'POST {{edgeUrl}}/auth/v3/oauth/token, Content-Type: application/x-www-form-urlencoded,\n      body grant_type=client_credentials&client_id=<id>&client_secret=<secret>'\n    response: '{\"access_token\": \"...\", \"expires_in\": 3600}'\n  - flow: password\n\
  \    grant: password\n    note: Password grant also documented for Litmus Edge / Litmus Unify.\n  usage: 'Send the access_token as Authorization: Bearer <token> on every call. Tokens\n    expire in 3600s; refresh before expiry. Do NOT call the Keycloak-style path.'\n- name: LitmusEdgeManagerAdminToken\n  type: apiKey\n  in: header\n  name_header: X-AuthToken\n  applies_to:\n  - Litmus Edge Manager\n  note: LEM uses an admin API token supplied in the X-AuthToken header. A /auth/validate\n    endpoint validates tokens.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/litmus-automation/refs/heads/main/authentication/litmus-automation-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Manufacturing
- Industrial IoT
- Edge Computing
- IIoT
- Unified Namespace
- MQTT
- DataOps
- Industrial Data Platform
- Analytics
---
