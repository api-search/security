---
api_key_in:
- query
- header
api_specs:
- filename: securden-password-retrieval-openapi.yml
  format: yaml
  label: Securden Password Retrieval API
  slug: securden-password-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securden/refs/heads/main/openapi/securden-password-retrieval-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Securden Authentication
name_suffix: Authentication
oauth_flows: []
overview: Securden secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Securden
provider_slug: securden
scheme_count: 1
schemes:
- description: Securden API Authentication Token. Static tokens are generated in the admin console (Admin >> API Access >> Authentication Token for APIs) and can be permanent or valid until a set date. Dynamic (short-lived) tokens are obtained programmatically. The CLI passes it as --authtoken alongside --server-url.
  in: query
  name: authtoken
  parameter: authtoken
  sources:
  - docs
  - packages/securden-packages.yml
  type: apiKey
slug: securden-authentication
source_filename: securden-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.securden.com/privileged-access-management/help/api-access/how-to-eliminate-hardcoded-credentials-using-apis-in-pam.html\ndocs: https://www.securden.com/privileged-access-management/help/api-access/how-to-eliminate-hardcoded-credentials-using-apis-in-pam.html\nsummary:\n  types: [apiKey]\n  api_key_in: [query, header]\n  oauth2_flows: []\n  notes: >-\n    Securden Unified PAM / Password Vault exposes a token-based REST API. Access is\n    regulated by an API Authentication Token created per API user/role. Both the official\n    Java client (ApiKeyAuth) and the securden-cli tool authenticate with an \"authtoken\".\nschemes:\n  - name: authtoken\n    type: apiKey\n    in: query\n    parameter: authtoken\n    description: >-\n      Securden API Authentication Token. Static tokens are generated in the admin\n      console (Admin >> API Access >> Authentication Token for APIs) and can be\n      permanent or valid until\
  \ a set date. Dynamic (short-lived) tokens are obtained\n      programmatically. The CLI passes it as --authtoken alongside --server-url.\n    sources: [docs, packages/securden-packages.yml]\ntoken_acquisition:\n  dynamic_token_endpoint: GET /api/get_auth_token\n  parameters: [login_name, password, domain_name]\n  example: 'curl -k -X GET \"https://{your_api_url}/api/get_auth_token?login_name=admin&password=admin&domain_name=xyz\"'\n  static_token: Admin >> API Access >> Authentication Token for APIs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/securden/refs/heads/main/authentication/securden-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Identity
- Security
- Privileged Access Management
- Password Management
- Secrets Management
- Endpoint Security
- DevOps
- AI Agent Security
---
