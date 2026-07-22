---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Nevis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nevis secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nevis
provider_slug: nevis
scheme_count: 1
schemes:
- description: REST API calls are authenticated with an "Access Key" created in the Authentication Cloud Management Console and sent on each request. The key scopes access to a single Authentication Cloud instance (tenant). The exact header parameter name is documented in the API endpoint reference.
  docs: https://docs.nevis.net/authcloud/getting-started/access-key
  in: header
  name: AccessKey
  sources:
  - docs.nevis.net/authcloud/getting-started/rest-api
  type: apiKey
slug: nevis-authentication
source_filename: nevis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  https://docs.nevis.net/authcloud/getting-started/access-key,\n  https://docs.nevis.net/authcloud/getting-started/rest-api — authentication\n  model for the Nevis Authentication Cloud REST API. Derived from the published\n  documentation rather than an OpenAPI securityScheme (Nevis does not publish a\n  machine-readable OpenAPI for the Authentication Cloud REST API).\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: AccessKey\n    type: apiKey\n    in: header\n    description: >-\n      REST API calls are authenticated with an \"Access Key\" created in the\n      Authentication Cloud Management Console and sent on each request. The key\n      scopes access to a single Authentication Cloud instance (tenant). The exact\n      header parameter name is documented in the API endpoint reference.\n    docs: https://docs.nevis.net/authcloud/getting-started/access-key\n    sources: [docs.nevis.net/authcloud/getting-started/rest-api]\n\
  notes: >-\n  End-user authentication is passwordless: FIDO2 / passkeys (Trusted key), the\n  Nevis Access App device authenticator (Trusted device), OATH TOTP, SMS OTP, and\n  recovery codes. The apiKey scheme above governs the server-to-server REST API,\n  not the end-user authentication ceremony.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nevis/refs/heads/main/authentication/nevis-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Authentication
- Identity
- Passwordless
- FIDO2
- Passkeys
- CIAM
- Transaction Signing
- Security
---
