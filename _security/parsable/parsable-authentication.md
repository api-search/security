---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Parsable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parsable secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Parsable
provider_slug: parsable
scheme_count: 2
schemes:
- description: 'User token obtained through the Authentication module login flow. Expires after 30 days. Passed on every request as `Authorization: Token <jwt>`.'
  expiry: 30d
  location: header
  name: StandardToken
  parameter: Authorization
  scheme: token
  token_format: JWT
  type: http
- description: 'Long-lived token for automated systems and server-to-server integrations. Does not expire on the 30-day standard schedule; allocated by Parsable on request. Passed as `Authorization: Token <jwt>`.'
  expiry: long-lived
  location: header
  name: PersistentToken
  parameter: Authorization
  scheme: token
  token_format: JWT
  type: http
slug: parsable-authentication
source_filename: parsable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://apidocs.parsable.com/\ndocs: https://apidocs.parsable.com/\nsummary:\n  types: [http]\n  http_schemes: [token]\n  token_format: JWT\n  header: Authorization\n  header_format: \"Token <jwt>\"\nschemes:\n  - name: StandardToken\n    type: http\n    scheme: token\n    token_format: JWT\n    description: >-\n      User token obtained through the Authentication module login flow. Expires after 30 days. Passed on\n      every request as `Authorization: Token <jwt>`.\n    location: header\n    parameter: Authorization\n    expiry: 30d\n  - name: PersistentToken\n    type: http\n    scheme: token\n    token_format: JWT\n    description: >-\n      Long-lived token for automated systems and server-to-server integrations. Does not expire on the\n      30-day standard schedule; allocated by Parsable on request. Passed as `Authorization: Token <jwt>`.\n    location: header\n    parameter: Authorization\n    expiry: long-lived\n\
  notes:\n  - All API calls are HTTP POST and must be made over SSL/TLS.\n  - \"Required headers include Authorization: Token <jwt>, Accept: application/json, and Wi-Thrift-Version: X.Y.Z.\"\n  - No OAuth2 / OpenID Connect discovery surface was found (/.well-known/openid-configuration returns 404).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parsable/refs/heads/main/authentication/parsable-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Connected Worker
- Manufacturing
- Industrial
- Digital Work Instructions
- Frontline Operations
- Workflow
- Analytics
---
