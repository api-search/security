---
api_key_in: []
api_specs:
- filename: methodfi-openapi-original.yml
  format: yaml
  label: Method API
  slug: method-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/methodfi/refs/heads/main/openapi/methodfi-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Methodfi Authentication
name_suffix: Authentication
oauth_flows: []
overview: MethodFi secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MethodFi
provider_slug: methodfi
scheme_count: 2
schemes:
- description: 'Secret key authentication. Use your team''s secret key (sk_...) as the Bearer

    token. All authenticated API endpoints require this scheme unless otherwise noted.

    This is the default/global security requirement across the OpenAPI.

    '
  format: Bearer sk_...
  header: Authorization
  in: header
  name: SecretKey
  scheme: bearer
  sources:
  - openapi/methodfi-openapi-original.yml
  type: http
- description: 'Opal token authentication for Opal session endpoints. Use an Opal token

    (otkn_...) as the Bearer token. Created via POST /opal/token using a secret key.

    '
  format: Bearer otkn_...
  header: Authorization
  in: header
  name: OpalToken
  scheme: bearer
  sources:
  - openapi/methodfi-openapi-original.yml
  type: http
slug: methodfi-authentication
source_filename: methodfi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/methodfi-openapi-original.yml\ndocs: https://docs.methodfi.com/2026-03-30/reference/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  token_prefixes:\n  - sk_    # secret key (server-side)\n  - pk_    # public key (client-side / Elements)\n  - otkn_  # Opal session token\n  notes: |\n    Method authenticates with API keys presented as HTTP Bearer tokens in the\n    Authorization header. Secret keys (sk_) authorize all server-side API calls;\n    public keys (pk_) are used for client-side Element/Opal requests; Opal session\n    tokens (otkn_) authorize Opal session endpoints. Every request must also send a\n    dated Method-Version header. Separate keys exist per environment (Development,\n    Sandbox, Production), managed in the Method Dashboard. No OAuth 2.0 / OIDC.\nschemes:\n- name: SecretKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer sk_...'\n\
  \  description: |\n    Secret key authentication. Use your team's secret key (sk_...) as the Bearer\n    token. All authenticated API endpoints require this scheme unless otherwise noted.\n    This is the default/global security requirement across the OpenAPI.\n  sources:\n  - openapi/methodfi-openapi-original.yml\n- name: OpalToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer otkn_...'\n  description: |\n    Opal token authentication for Opal session endpoints. Use an Opal token\n    (otkn_...) as the Bearer token. Created via POST /opal/token using a secret key.\n  sources:\n  - openapi/methodfi-openapi-original.yml\nextras:\n  version_header:\n    name: Method-Version\n    required: true\n    current: '2026-03-30'\n    example: '2026-03-30'\n  ip_whitelisting:\n    supported: true\n    docs: https://docs.methodfi.com/2026-03-30/reference/ip-whitelisting\n  message_level_encryption:\n    supported: true\n    docs: https://docs.methodfi.com/2026-03-30/reference/message-level-encryption\n\
  \    jwks: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/methodfi/refs/heads/main/authentication/methodfi-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Fintech
- Liability Data
- Payments
- Lending
- Personal Finance
- Credit
- ACH
- Debt
- Identity Verification
---
