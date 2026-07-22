---
api_key_in:
- header
auth_types:
- http-basic
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Nova Credit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nova Credit secures its APIs with http-basic and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nova Credit
provider_slug: nova-credit
scheme_count: 2
schemes:
- applies_to:
  - GET /connect/accesstoken
  description: 'Base64-encoded clientId:secretKey passed as `Authorization: Basic <creds>` to obtain an access token from GET /connect/accesstoken.'
  name: BasicAuth
  scheme: basic
  sources:
  - https://docs.novacredit.com/credit-passport/v4
  type: http
- applies_to:
  - GET /connect/passport/v4/json
  - GET /connect/passport/v4/pdf
  - GET /connect/status
  bearer_format: opaque
  description: 'Short-lived accessToken (5 minute lifetime) passed as `Authorization: Bearer <accessToken>` to retrieve reports and call server-side endpoints.'
  name: BearerAuth
  scheme: bearer
  sources:
  - https://docs.novacredit.com/credit-passport/v4
  type: http
slug: nova-credit-authentication
source_filename: nova-credit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.novacredit.com/credit-passport/v4\ndocs: https://docs.novacredit.com/credit-passport-quickstart\nsummary:\n  types: [http-basic, http-bearer]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Two-step credential model. Server-side clients authenticate to the token\n    endpoint with HTTP Basic using base64(clientId:secretKey), receive a\n    short-lived (5 minute) accessToken, then call report/data endpoints with an\n    HTTP Bearer accessToken. Report payloads are additionally JWE-encrypted using\n    RSA-OAEP-256; consumers fetch Nova Credit's RSA public keys from a JWKS\n    endpoint. Client-side (NovaConnect / webview) integrations are identified by a\n    publicId rather than the secret key.\nschemes:\n  - name: BasicAuth\n    type: http\n    scheme: basic\n    description: >-\n      Base64-encoded clientId:secretKey passed as `Authorization: Basic <creds>`\n      to obtain an access token from\
  \ GET /connect/accesstoken.\n    applies_to: [GET /connect/accesstoken]\n    sources: [https://docs.novacredit.com/credit-passport/v4]\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    bearer_format: opaque\n    description: >-\n      Short-lived accessToken (5 minute lifetime) passed as\n      `Authorization: Bearer <accessToken>` to retrieve reports and call\n      server-side endpoints.\n    applies_to:\n      - GET /connect/passport/v4/json\n      - GET /connect/passport/v4/pdf\n      - GET /connect/status\n    sources: [https://docs.novacredit.com/credit-passport/v4]\ncredentials:\n  - name: publicId\n    role: client-side account identifier (NovaConnect / webview)\n  - name: clientId\n    role: server-side API identifier (Basic Auth username)\n  - name: secretKey\n    role: server-side API secret (Basic Auth password) — confidential\n  - name: publicToken\n    role: identifies a specific Credit Passport report\n  - name: accessToken\n    role: short-lived (5 min) bearer\
  \ token authorizing server-side requests\nrequest_headers:\n  - name: X-PUBLIC-TOKEN\n    description: Report identifier for report-retrieval requests\n  - name: X-EXTERNAL-ID\n    description: Caller-supplied applicant identifier\n  - name: X-PUBLIC-ID\n    description: Required when using X-EXTERNAL-ID with Parent accounts\npayload_encryption:\n  scheme: JWE\n  algorithm: RSA-OAEP-256\n  key_use: enc\n  jwks_endpoint: https://api.novacredit.com/connect/jwkset\n  verified_status: 200\nenterprise_identity:\n  scim: https://docs.novacredit.com/scim\n  sso: https://docs.novacredit.com/sso\nenvironments:\n  production: https://api.novacredit.com\n  sandbox: https://api.sandbox.novacredit.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nova-credit/refs/heads/main/authentication/nova-credit-authentication.yml
summary_line: http-basic/http-bearer · 2 schemes
tags:
- Company
- Credit Data
- Consumer Credit
- Credit Bureau
- Income Verification
- Underwriting
- Fintech
- Financial Services
- Lending
- Cash Flow Underwriting
- Identity
---
