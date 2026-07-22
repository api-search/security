---
api_key_in:
- signature
auth_types:
- signedRequest
- bearer
description: ''
kind: authentication
layout: security
method: searched
name: Urbanlogiq Authentication
name_suffix: Authentication
oauth_flows: []
overview: UrbanLogiq secures its APIs with signedRequest and bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: UrbanLogiq
provider_slug: urbanlogiq
scheme_count: 2
schemes:
- description: All access to UrbanLogiq systems requires authentication, typically with signed requests using API keys. An API key consists of an Access Key ID and a Secret Key; the Secret Key signs a canonical request (method, path, sorted query string, signed headers, SHA-256 body hash — an AWS SigV4-style canonicalization) with an Ed25519 signature carried as X-UL-Signature. Keys are bound to a user ID (UUID), a region (US or CA), and an environment (prod or stage), and can be stored in profile form in a local ~/.ul/keys file.
  key_portal:
  - region: us
    url: https://home.urbanlogiq.us/admin/keys
  - region: ca
    url: https://home.urbanlogiq.ca/admin/keys
  name: UL1-ED25519
  request_type: ul1_request
  signature: UL1-ED25519
  signature_header: X-UL-Signature
  sources:
  - https://github.com/urbanlogiq/ulsdk
  type: signedRequest
  verification_call: GET /v1/bootstrap/ (api.gate.bootstrap returns current user, groups, client secrets)
- description: The SDK RequestContext abstraction also supports bearer-token authentication as an alternative to signed requests (used by the web application session flow).
  name: bearer
  scheme: bearer
  sources:
  - https://github.com/urbanlogiq/ulsdk
  type: http
slug: urbanlogiq-authentication
source_filename: urbanlogiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/urbanlogiq/ulsdk\ndocs: https://github.com/urbanlogiq/ulsdk#authentication\nsummary:\n  types: [signedRequest, bearer]\n  api_key_in: [signature]\n  oauth2_flows: []\nschemes:\n- name: UL1-ED25519\n  type: signedRequest\n  description: >-\n    All access to UrbanLogiq systems requires authentication, typically with\n    signed requests using API keys. An API key consists of an Access Key ID\n    and a Secret Key; the Secret Key signs a canonical request (method, path,\n    sorted query string, signed headers, SHA-256 body hash — an AWS\n    SigV4-style canonicalization) with an Ed25519 signature carried as\n    X-UL-Signature. Keys are bound to a user ID (UUID), a region (US or CA),\n    and an environment (prod or stage), and can be stored in profile form in\n    a local ~/.ul/keys file.\n  signature: UL1-ED25519\n  signature_header: X-UL-Signature\n  request_type: ul1_request\n  key_portal:\n  - region:\
  \ us\n    url: https://home.urbanlogiq.us/admin/keys\n  - region: ca\n    url: https://home.urbanlogiq.ca/admin/keys\n  verification_call: GET /v1/bootstrap/ (api.gate.bootstrap returns current user, groups, client secrets)\n  sources: [https://github.com/urbanlogiq/ulsdk]\n- name: bearer\n  type: http\n  scheme: bearer\n  description: >-\n    The SDK RequestContext abstraction also supports bearer-token\n    authentication as an alternative to signed requests (used by the web\n    application session flow).\n  sources: [https://github.com/urbanlogiq/ulsdk]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urbanlogiq/refs/heads/main/authentication/urbanlogiq-authentication.yml
summary_line: signedRequest/bearer · 2 schemes
tags:
- Company
- Government
- GovTech
- Data
- Analytics
- Transportation
- Urban Planning
- Public Safety
- Economic Development
- Artificial Intelligence
---
