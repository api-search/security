---
api_key_in:
- query
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Infutor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Infutor secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Infutor
provider_slug: infutor
scheme_count: 3
schemes:
- example: https://api.leadid.com/Authenticate?lac={ACCOUNTCODE}&id={LEADIDTOKEN}
  in: query
  name: leadidQueryCredentials
  parameters:
  - description: Account Code (UUID) issued by InfutorData / LeadiD.
    name: lac
    required: true
  - description: LeadiD token to authenticate/audit (UUID); may be optional when "LeadiD Optional" is enabled.
    name: id
    required: false
  source: https://help.infutor.com/apidocs/endpoint-for-a-lead-audit.md
  type: apiKey
- description: Optional Bearer token in the Authorization header, required when API Authentication is enabled on the LeadiD query endpoints (e.g. /SingleQuery).
  header: Authorization
  in: header
  name: bearerToken
  scheme: bearer
  source: https://help.infutor.com/apidocs/endpoint-for-a-lead-audit.md
  type: http
- description: The Audit / Intelligence API requires a customer-supplied `authorization` request header carrying the token(s) InfutorData generates for the account.
  header: authorization
  in: header
  name: audit_authorization_token
  source: https://help.infutor.com/docs/infutor-api.md
  type: apiKey
slug: infutor-authentication
source_filename: infutor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://help.infutor.com/docs/authentication-api.md\ndocs: https://help.infutor.com/docs/infutor-api.md\nsummary:\n  types: [apiKey, http]\n  api_key_in: [query, header]\n  oauth2_flows: []\n  notes: >-\n    InfutorData / LeadiD (part of ActiveProspect) uses account-code + LeadiD-token\n    query-parameter credentials on the LeadiD query APIs, plus an optional HTTP\n    Bearer token in the Authorization header when API Authentication is enabled.\n    The Audit/Intelligence API additionally documents a customer-supplied\n    `authorization: {token}` request header carrying InfutorData-generated tokens.\nschemes:\n  - name: leadidQueryCredentials\n    type: apiKey\n    in: query\n    parameters:\n      - name: lac\n        description: Account Code (UUID) issued by InfutorData / LeadiD.\n        required: true\n      - name: id\n        description: LeadiD token to authenticate/audit (UUID); may be optional when \"LeadiD Optional\"\
  \ is enabled.\n        required: false\n    source: https://help.infutor.com/apidocs/endpoint-for-a-lead-audit.md\n    example: https://api.leadid.com/Authenticate?lac={ACCOUNTCODE}&id={LEADIDTOKEN}\n  - name: bearerToken\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    description: >-\n      Optional Bearer token in the Authorization header, required when API\n      Authentication is enabled on the LeadiD query endpoints (e.g. /SingleQuery).\n    source: https://help.infutor.com/apidocs/endpoint-for-a-lead-audit.md\n  - name: audit_authorization_token\n    type: apiKey\n    in: header\n    header: authorization\n    description: >-\n      The Audit / Intelligence API requires a customer-supplied `authorization`\n      request header carrying the token(s) InfutorData generates for the account.\n    source: https://help.infutor.com/docs/infutor-api.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infutor/refs/heads/main/authentication/infutor-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Identity Resolution
- Consumer Data
- Data Enrichment
- Lead Verification
- TCPA Compliance
- Marketing
- Identity
---
