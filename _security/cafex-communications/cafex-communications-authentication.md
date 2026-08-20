---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cafex Communications Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: CafeX Communications secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: CafeX Communications
provider_slug: cafex-communications
scheme_count: 2
schemes:
- flow: clientCredentials
  name: cafexOAuth2ClientCredentials
  parameters:
  - name: grant_type
    required: true
    value: client_credentials
  - name: client_id
    note: issued in the CafeX tenant UI under Tenant settings > Management > Client applications
    required: true
  - name: client_secret
    required: true
  request_content_type: application/x-www-form-urlencoded
  response_field: access_token
  scopes: []
  scopes_note: The published documentation declares no scope parameter and no scope values.
  sources:
  - https://support.cafex.com/support/solutions/articles/73000645442-accessing-audit-information-programmatically
  token_lifetime: 8h
  token_url: https://auth.cafex.com/authserver/token
  type: oauth2
- applies_to:
  - https://app.cafex.com/audit-search-rest/search
  format: Bearer {ACCESS TOKEN HERE}
  header: Authorization
  in: header
  name: cafexBearer
  scheme: bearer
  sources:
  - https://support.cafex.com/support/solutions/articles/73000645442-accessing-audit-information-programmatically
  type: http
slug: cafex-communications-authentication
source_filename: cafex-communications-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: searched\nsource: https://support.cafex.com/support/solutions/articles/73000645442-accessing-audit-information-programmatically\ndocs: https://support.cafex.com/support/solutions/articles/73000645442-accessing-audit-information-programmatically\nnote: >-\n  CafeX publishes no OpenAPI document, so this profile is transcribed from the published\n  Audit Events API documentation and confirmed against live anonymous probes of both\n  endpoints. No securityScheme could be derived mechanically.\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\n  bearer_format: opaque access_token\nschemes:\n- name: cafexOAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://auth.cafex.com/authserver/token\n  request_content_type: application/x-www-form-urlencoded\n  parameters:\n  - name: grant_type\n    value: client_credentials\n    required: true\n  - name: client_id\n    required:\
  \ true\n    note: issued in the CafeX tenant UI under Tenant settings > Management > Client applications\n  - name: client_secret\n    required: true\n  response_field: access_token\n  token_lifetime: 8h\n  scopes: []\n  scopes_note: The published documentation declares no scope parameter and no scope values.\n  sources:\n  - https://support.cafex.com/support/solutions/articles/73000645442-accessing-audit-information-programmatically\n- name: cafexBearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer {ACCESS TOKEN HERE}'\n  applies_to:\n  - https://app.cafex.com/audit-search-rest/search\n  sources:\n  - https://support.cafex.com/support/solutions/articles/73000645442-accessing-audit-information-programmatically\ncredential_issuance:\n  self_service: false\n  path: CafeX tenant UI > three-dot header menu > Tenant settings > Management > Client applications > Add\n  note: >-\n    Client applications are created by a tenant administrator inside the\
  \ authenticated CafeX\n    product; there is no anonymous developer sign-up that yields API credentials.\nin_product_credentials:\n  note: >-\n    Separately from the platform's own API, CafeX App Studio external data sources support\n    per-user stored credentials for OUTBOUND calls to third-party APIs — OAuth (clientId /\n    clientSecret / tokenUrl), custom auth headers, and HTTP Basic. These are consumer-side\n    credential slots, not authentication to a CafeX API.\n  docs: https://support.cafex.com/support/solutions/articles/73000657127-setting-up-client-credentials\nx-evidence:\n- url: https://auth.cafex.com/authserver/token\n  method: POST\n  http_status: 400\n  fetched: '2026-08-08'\n  body: '{\"error\":\"invalid_client\",\"error_description\":\"Client ID or the Client secret are invalid\"}'\n  note: anonymous probe; live OAuth 2.0 token endpoint confirmed\n- url: https://app.cafex.com/audit-search-rest/search\n  method: POST\n  http_status: 400\n  fetched: '2026-08-08'\n  note:\
  \ anonymous probe with an empty JSON body; live REST endpoint confirmed\n- url: https://auth.cafex.com/.well-known/openid-configuration\n  http_status: 404\n  fetched: '2026-08-08'\n  note: no OIDC discovery document\n- url: https://auth.cafex.com/.well-known/oauth-authorization-server\n  http_status: 404\n  fetched: '2026-08-08'\n  note: no RFC 8414 authorization-server metadata\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cafex-communications/refs/heads/main/authentication/cafex-communications-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Low-Code
- Workflow-Automation
- Agentic AI
- Audit and Compliance
- Collaboration
- Enterprise Software
- Regulated Industries
- Process Automation
---
