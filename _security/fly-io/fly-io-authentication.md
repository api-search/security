---
api_key_in:
- header
api_specs:
- filename: fly-io-machines-api-openapi.yml
  format: yaml
  label: Fly.io Machines API
  slug: machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fly-io/refs/heads/main/openapi/fly-io-machines-api-openapi.yml
- filename: fly-io-extensions-api-openapi.yml
  format: yaml
  label: Fly.io Extensions API
  slug: extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fly-io/refs/heads/main/openapi/fly-io-extensions-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fly Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: fly-io secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: fly-io
provider_slug: fly-io
scheme_count: 2
schemes:
- description: Shared secret provided by Fly.io to the extension provider. Fly.io includes this secret in an Authorization Bearer header on all requests to the provider's API for verification.
  name: flySharedSecret
  scheme: bearer
  sources:
  - openapi/fly-io-extensions-api-openapi.yml
  - openapi/fly-io-machines-api-openapi.yml
  type: http
- description: HMAC-SHA256 signature of the raw request body, computed using the webhook signing secret. Recipients must verify this signature before processing the payload.
  in: header
  name: webhookHmac
  parameter: X-Fly-Signature
  sources:
  - openapi/fly-io-extensions-api-openapi.yml
  type: apiKey
slug: fly-io-authentication
source_filename: fly-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fly-io-extensions-api-openapi.yml, openapi/fly-io-machines-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: flySharedSecret\n  type: http\n  scheme: bearer\n  description: Shared secret provided by Fly.io to the extension provider. Fly.io includes this\n    secret in an Authorization Bearer header on all requests to the provider's API for verification.\n  sources:\n  - openapi/fly-io-extensions-api-openapi.yml\n  - openapi/fly-io-machines-api-openapi.yml\n- name: webhookHmac\n  type: apiKey\n  in: header\n  parameter: X-Fly-Signature\n  description: HMAC-SHA256 signature of the raw request body, computed using the webhook signing\n    secret. Recipients must verify this signature before processing the payload.\n  sources:\n  - openapi/fly-io-extensions-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fly-io/refs/heads/main/authentication/fly-io-authentication.yml
summary_line: apiKey/http · 2 schemes
tags: []
---
