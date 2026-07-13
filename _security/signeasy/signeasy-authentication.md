---
api_key_in: []
api_specs:
- filename: signeasy-openapi.yml
  format: yaml
  label: Signeasy Envelopes API
  slug: signeasy-envelopes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signeasy/refs/heads/main/openapi/signeasy-openapi.yml
- filename: signeasy-openapi.yml
  format: yaml
  label: Signeasy Originals API
  slug: signeasy-originals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signeasy/refs/heads/main/openapi/signeasy-openapi.yml
- filename: signeasy-openapi.yml
  format: yaml
  label: Signeasy Templates API
  slug: signeasy-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signeasy/refs/heads/main/openapi/signeasy-openapi.yml
- filename: signeasy-openapi.yml
  format: yaml
  label: Signeasy Embedded Signing API
  slug: signeasy-embedded-signing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signeasy/refs/heads/main/openapi/signeasy-openapi.yml
- filename: signeasy-openapi.yml
  format: yaml
  label: Signeasy Webhooks API
  slug: signeasy-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signeasy/refs/heads/main/openapi/signeasy-openapi.yml
- filename: signeasy-openapi.yml
  format: yaml
  label: Signeasy Users API
  slug: signeasy-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signeasy/refs/heads/main/openapi/signeasy-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Signeasy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Signeasy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Signeasy
provider_slug: signeasy
scheme_count: 1
schemes:
- description: OAuth 2.0 access token (sandbox or live) passed as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/signeasy-openapi.yml
  type: http
slug: signeasy-authentication
source_filename: signeasy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/signeasy-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token (sandbox or live) passed as a Bearer token in the Authorization\n    header.\n  sources:\n  - openapi/signeasy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signeasy/refs/heads/main/authentication/signeasy-authentication.yml
summary_line: http · 1 scheme
tags:
- eSignature
- Electronic Signature
- Documents
- Contract Management
- Embedded Signing
- Templates
- Webhooks
---
