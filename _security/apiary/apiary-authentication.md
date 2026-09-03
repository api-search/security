---
api_key_in:
- header
api_specs:
- filename: apiary-apiary-api-openapi.yml
  format: yaml
  label: Apiary API
  slug: apiary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiary/refs/heads/main/openapi/apiary-apiary-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Apiary Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apiary secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Apiary
provider_slug: apiary
scheme_count: 3
schemes:
- description: HTTP Basic authentication with the Apiary account email and password. Used only on /authorization to mint, list and revoke tokens. Not available to users in IDCS-controlled teams.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/apiary-apiary-api-openapi.yml
  type: http
- description: 'RFC 6750 Bearer token. Generate at https://login.apiary.io/tokens or via POST /authorization. Sent as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/apiary-apiary-api-openapi.yml
  type: http
- description: 'Legacy Apiary token header, sent as `Authentication: Token <token>` (note: the header is `Authentication`, not `Authorization`). Apiary labels the /blueprint/* group legacy. This is the same token value the Apiary CLI reads from the APIARY_API_KEY environment variable.'
  in: header
  name: legacyToken
  parameter: Authentication
  sources:
  - openapi/apiary-apiary-api-openapi.yml
  type: apiKey
slug: apiary-authentication
source_filename: apiary-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: openapi/apiary-apiary-api-openapi.yml\ndocs: https://apiary.docs.apiary.io\ndocs_detail: >-\n  Upgraded from derived to searched on 2026-09-02 after reading Apiary's own\n  published authentication documentation: the Authentication and User Information\n  resource-group descriptions in https://jsapi.apiary.io/apis/apiary (which cite\n  RFC 6750 directly and give worked Basic-auth and Bearer curl examples), plus\n  https://help.apiary.io/tools/apiary-cli/ for the APIARY_API_KEY environment\n  variable and https://login.apiary.io/tokens for token issuance.\nnotes:\n  - >-\n    THE HEADER NAME IS NOT UNIFORM. /me and /me/apis take `Authorization: Bearer`;\n    /blueprint/* takes `Authentication: Token` — a different header, same token\n    value. Apiary calls the second one legacy.\n  - >-\n    Tokens are unscoped and account-wide. There are no OAuth scopes, no read-only\n    tokens and no per-project tokens; Apiary documents\
  \ the token as equivalent to a\n    password.\n  - >-\n    The /authorization resource uses HTTP Basic with the account email and password,\n    and does NOT work for users who are part of Oracle IDCS-controlled teams.\n  - >-\n    An invalid Bearer token is answered 401 with `WWW-Authenticate: Bearer\n    error=\"invalid_token\"` — RFC 6750 conformant challenge signalling.\n  - No token expiry, refresh, rotation window or last-used metadata is published.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication with the Apiary account email and password. Used only\n    on /authorization to mint, list and revoke tokens. Not available to users in IDCS-controlled\n    teams.\n  sources:\n  - openapi/apiary-apiary-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'RFC 6750 Bearer token. Generate at https://login.apiary.io/tokens or via POST\n \
  \   /authorization. Sent as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/apiary-apiary-api-openapi.yml\n- name: legacyToken\n  type: apiKey\n  in: header\n  parameter: Authentication\n  description: 'Legacy Apiary token header, sent as `Authentication: Token <token>` (note: the\n    header is `Authentication`, not `Authorization`). Apiary labels the /blueprint/* group legacy.\n    This is the same token value the Apiary CLI reads from the APIARY_API_KEY environment variable.'\n  sources:\n  - openapi/apiary-apiary-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiary/refs/heads/main/authentication/apiary-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- API Blueprint
- API Design
- API Testing
- Collaboration
- Design-First
- Documentation
- Mock Servers
- Oracle
---
