---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Jifflenow Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Jifflenow secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Jifflenow
provider_slug: jifflenow
scheme_count: 2
schemes:
- flow: clientCredentials
  name: OAuth2 Client Credentials
  parameters:
  - grant_type=client_credentials
  - client_id
  - client_secret
  sources:
  - https://developers.cvent.com/docs/legacy-api/jifflenow-api/getting-started
  status: recommended
  token_request_content_type: application/x-www-form-urlencoded
  token_response_fields:
  - access_token
  - token_type
  - expires_in
  - scope
  - created_at
  token_ttl_seconds: 1800
  token_type: Bearer
  token_url: https://<companyname>.jifflenow.com/api/oauth/token
  type: oauth2
  usage_header: 'Authorization: Bearer <ACCESS_TOKEN>'
- flow: authorizationCode
  name: OAuth2 Authorization Code (legacy)
  note: The docs state "Authorization Code Grant is deprecated. All new integrations should use the Client Credentials Flow." The authorization-code flow additionally requires an X-Integration-User-Id request header naming the integration user; the client-credentials flow does not.
  sources:
  - https://developers.cvent.com/docs/legacy-api/jifflenow-api/getting-started
  status: deprecated
  type: oauth2
slug: jifflenow-authentication
source_filename: jifflenow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.cvent.com/docs/legacy-api/jifflenow-api/getting-started\ndocs: https://developers.cvent.com/docs/legacy-api/jifflenow-api/getting-started\nnote: >-\n  Jifflenow was acquired by Cvent in 2021. jifflenow.com now 302s to the Cvent product page, but the\n  Jifflenow REST API is still live and publicly documented on the acquirer's developer portal at\n  developers.cvent.com/docs/legacy-api/jifflenow-api/. The API host remains Jifflenow's own domain\n  (https://<companyname>.jifflenow.com/api), which is why this profile — not the Cvent profile —\n  carries the artifact. No OpenAPI is published for this API; everything below is read from the\n  human documentation.\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [clientCredentials, authorizationCode]\nschemes:\n  - name: OAuth2 Client Credentials\n    type: oauth2\n    flow: clientCredentials\n    status: recommended\n    token_url: https://<companyname>.jifflenow.com/api/oauth/token\n\
  \    token_request_content_type: application/x-www-form-urlencoded\n    parameters:\n      - grant_type=client_credentials\n      - client_id\n      - client_secret\n    token_response_fields: [access_token, token_type, expires_in, scope, created_at]\n    token_type: Bearer\n    token_ttl_seconds: 1800\n    usage_header: 'Authorization: Bearer <ACCESS_TOKEN>'\n    sources: [https://developers.cvent.com/docs/legacy-api/jifflenow-api/getting-started]\n  - name: OAuth2 Authorization Code (legacy)\n    type: oauth2\n    flow: authorizationCode\n    status: deprecated\n    note: >-\n      The docs state \"Authorization Code Grant is deprecated. All new integrations should use the\n      Client Credentials Flow.\" The authorization-code flow additionally requires an\n      X-Integration-User-Id request header naming the integration user; the client-credentials flow\n      does not.\n    sources: [https://developers.cvent.com/docs/legacy-api/jifflenow-api/getting-started]\nrequest_headers:\n\
  \  - name: Authorization\n    required: true\n    value: Bearer {access_token}\n  - name: X-Integration-User-Id\n    required: conditional\n    value: UUID of the integration user\n    note: Required only with the deprecated authorization-code flow, not with client credentials.\ncredential_issuance:\n  self_service: false\n  path: >-\n    Settings (Company Homepage) -> Integrations -> + New Integration -> \"Jifflenow REST APIs\".\n    The side panel exposes Client ID, Client Secret and Subdomain. Requires the \"Can manage\n    integrations\" privilege inside a Jifflenow tenant.\n  per_event_activation: 'Event > Settings > Integrations'\n  support_contact: jn-support@cvent.com\n  docs: https://developers.cvent.com/docs/legacy-api/jifflenow-api/getting-started\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jifflenow/refs/heads/main/authentication/jifflenow-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Automation
- Event
- Meetings
- Scheduling
- Event Marketing
- B2B
- Sales
- Trade Shows
- Meeting Automation
- Appointments
- Badge Scanning
---
