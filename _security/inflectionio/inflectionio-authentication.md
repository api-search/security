---
api_key_in: []
api_specs:
- filename: inflectionio-openapi-original.yml
  format: yaml
  label: Inflection Developer API
  slug: inflectionio-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflectionio/refs/heads/main/openapi/inflectionio-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Inflectionio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Inflection.io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Inflection.io
provider_slug: inflectionio
scheme_count: 1
schemes:
- description: 'Personal Access Token sent as a bearer credential (Authorization: Bearer [example key]). Tokens are scoped READ (required for every GET) and WRITE (required for POST/PATCH/DELETE).'
  failures:
    '401': Missing, malformed, or invalid token (also returned for unknown paths/methods under /v1, deny-by-default).
    '403': Token is valid but lacks the required scope (e.g. a READ token attempting a write).
  name: bearerAuth
  notes: Gateway auth errors (401/403) return an empty body; the status code carries the meaning.
  scheme: bearer
  scopes:
  - description: Required for every GET request.
    name: READ
  - description: Required for POST, PATCH, and DELETE requests.
    name: WRITE
  sources:
  - openapi/inflectionio-openapi-original.yml
  token_prefix: inf_pat_
  type: http
slug: inflectionio-authentication
source_filename: inflectionio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/inflectionio-openapi-original.yml\ndocs: https://github.com/inflectionio/mintlify-docs/blob/develop/api-reference/authentication.mdx\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  token_type: personal-access-token\n  token_prefix: inf_pat_\n  scopes:\n  - READ\n  - WRITE\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Personal Access Token sent as a bearer credential (Authorization: Bearer [example key]).\n    Tokens are scoped READ (required for every GET) and WRITE (required for POST/PATCH/DELETE).\n  token_prefix: inf_pat_\n  scopes:\n  - name: READ\n    description: Required for every GET request.\n  - name: WRITE\n    description: Required for POST, PATCH, and DELETE requests.\n  failures:\n    '401': Missing, malformed, or invalid token (also returned for unknown paths/methods under /v1, deny-by-default).\n    '403': Token is valid but lacks the required scope\
  \ (e.g. a READ token attempting a write).\n  notes: Gateway auth errors (401/403) return an empty body; the status code carries the meaning.\n  sources:\n  - openapi/inflectionio-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inflectionio/refs/heads/main/authentication/inflectionio-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Saas
- Marketing
- Marketing Automation
- Email Marketing
- Customer Data
- B2B
- Contacts
- API
---
