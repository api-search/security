---
api_key_in: []
api_specs:
- filename: hellosign-openapi-original.yaml
  format: yaml
  label: Dropbox Sign API
  slug: dropbox-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-openapi-original.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Hellosign Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dropbox Sign (HelloSign) secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dropbox Sign (HelloSign)
provider_slug: hellosign
scheme_count: 2
schemes:
- description: 'Your API key can be used to make calls to the Dropbox Sign API. See [Authentication](/api/reference/authentication) for more information.

    ✅ Supported by Try it console (calls sent in `test_mode` only).'
  name: api_key
  scheme: basic
  sources:
  - openapi/hellosign-openapi-original.yaml
  type: http
- bearerFormat: JWT
  description: 'You can use an Access Token issued through an OAuth flow to send calls to the Dropbox Sign API from your app. The access scopes required by this endpoint are listed in the gray box above. See [Authentication](/api/reference/authentication) for more information.

    ❌ **Not supported** by Try it console.'
  name: oauth2
  scheme: bearer
  sources:
  - openapi/hellosign-openapi-original.yaml
  type: http
slug: hellosign-authentication
source_filename: hellosign-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/hellosign-openapi-original.yaml\ndocs: https://developers.hellosign.com/api/reference/authentication/\nsummary:\n  types:\n  - http\n  api_key_style: http-basic (API key as Basic username, empty password)\n  oauth2_flow: authorizationCode\n  oauth2_authorization_url: https://app.hellosign.com/oauth/authorize\n  oauth2_token_url: https://app.hellosign.com/oauth/token\n  scopes_artifact: scopes/hellosign-scopes.yml\nschemes:\n- name: api_key\n  type: http\n  scheme: basic\n  description: |-\n    Your API key can be used to make calls to the Dropbox Sign API. See [Authentication](/api/reference/authentication) for more information.\n    ✅ Supported by Try it console (calls sent in `test_mode` only).\n  sources:\n  - openapi/hellosign-openapi-original.yaml\n- name: oauth2\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    You can use an Access Token issued through an OAuth flow to send calls to\
  \ the Dropbox Sign API from your app. The access scopes required by this endpoint are listed in the gray box above. See [Authentication](/api/reference/authentication) for more information.\n    ❌ **Not supported** by Try it console.\n  sources:\n  - openapi/hellosign-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/authentication/hellosign-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- eSignature
- Electronic Signatures
- Documents
- Digital Agreements
- Signature Workflow
- Embedded Signing
- Compliance
---
