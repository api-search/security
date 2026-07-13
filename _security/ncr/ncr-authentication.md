---
api_key_in:
- header
api_specs:
- filename: ncr-voyix-commerce-platform-openapi.yml
  format: yaml
  label: NCR Voyix Commerce Platform APIs
  slug: ncr-voyix-commerce-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncr/refs/heads/main/openapi/ncr-voyix-commerce-platform-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ncr Authentication
name_suffix: Authentication
oauth_flows: []
overview: NCR secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NCR
provider_slug: ncr
scheme_count: 1
schemes:
- description: 'AccessKey (HMAC) authentication. The Authorization header carries "AccessKey {sharedKey}:{signature}", where the signature is a Base64 SHA-512 HMAC computed over the HTTP method, encoded request path and query string, Content-Type, optional Content-MD5, optional nep-application-key, and optional nep-correlation-id, keyed by the secret key concatenated with the ISO-8601 request date. A Date header '
  in: header
  name: hmacAccessKey
  parameter: Authorization
  sources:
  - openapi/ncr-voyix-commerce-platform-openapi.yml
  type: apiKey
slug: ncr-authentication
source_filename: ncr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ncr-voyix-commerce-platform-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmacAccessKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'AccessKey (HMAC) authentication. The Authorization header carries \"AccessKey\n    {sharedKey}:{signature}\", where the signature is a Base64 SHA-512 HMAC computed over the\n    HTTP method, encoded request path and query string, Content-Type, optional Content-MD5,\n    optional nep-application-key, and optional nep-correlation-id, keyed by the secret key concatenated\n    with the ISO-8601 request date. A Date header '\n  sources:\n  - openapi/ncr-voyix-commerce-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ncr/refs/heads/main/authentication/ncr-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Restaurant
- Retail
- Banking
- ATM
- Point of Sale
- Commerce
- Fortune 500
---
