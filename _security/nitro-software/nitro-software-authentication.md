---
api_key_in: []
api_specs:
- filename: nitro-software-openapi-original.json
  format: json
  label: Nitro API (Sign + PDF Services)
  slug: nitro-api-sign-pdf-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nitro-software/refs/heads/main/openapi/nitro-software-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Nitro Software Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Nitro Software secures its APIs with http and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Nitro Software
provider_slug: nitro-software
scheme_count: 1
schemes:
- applied_to: all /sign/* and /transformations,/generations,/extractions,/conversions,/jobs operations
  bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nitro-software-openapi-original.json
  type: http
slug: nitro-software-authentication
source_filename: nitro-software-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/nitro-software-openapi-original.json\ndocs: https://developers.gonitro.com/docs/authentication/credentials\nsummary:\n  types:\n  - http\n  - oauth2\n  model: machine-to-machine OAuth 2.0 client-credentials grant issuing short-lived bearer JWTs\n  api_key_in: []\n  oauth2_flows:\n  - clientCredentials\noauth2:\n  grant_type: client_credentials\n  token_endpoint: https://api.gonitro.dev/oauth/token\n  request_body:\n    clientID: '<nitro_app_id>'\n    clientSecret: '<your_app_secret>'\n  token_response:\n    accessToken: JWT\n    tokenType: Bearer\n    expiresIn: 86400\n  notes: >-\n    Credentials (Client ID + Client Secret + OAuth token endpoint) are issued per application\n    in the Nitro Admin Portal (admin.gonitro.com); up to 25 applications per account. API\n    access requires a Nitro Sign Enterprise plan. Tokens should be cached to their expiresIn\n    and renewed on 401. No OAuth scopes are declared — access\
  \ is application/tenant scoped.\n    Credentials can be rotated immediately from the Admin Portal to revoke a compromised secret.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applied_to: all /sign/* and /transformations,/generations,/extractions,/conversions,/jobs operations\n  sources:\n  - openapi/nitro-software-openapi-original.json\nextra_headers:\n- name: nitro-guest-id\n  note: guest-scoped access header (403 when invalid/expired) for guest signer flows\ncredential_rotation:\n  docs: https://developers.gonitro.com/docs/authentication/credential-rotation\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nitro-software/refs/heads/main/authentication/nitro-software-authentication.yml
summary_line: http/oauth2 · 1 scheme
tags:
- Company
- PDF
- Documents
- eSignature
- Electronic Signature
- Document Management
- Document Intelligence
- OCR
- Data Extraction
- Productivity
---
