---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: ParseForMe API
  slug: parseforme-api
  spec_type: OpenAPI
  url: https://api.parseforme.com/v1/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Parseforme Authentication
name_suffix: Authentication
oauth_flows: []
overview: ParseForMe secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ParseForMe
provider_slug: parseforme
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: A `pfm_live_…` workspace key
  name: bearer
  scheme: bearer
  sources:
  - openapi/parseforme-openapi-original.json
  type: http
slug: parseforme-authentication
source_filename: parseforme-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: openapi/parseforme-openapi-original.json\ndocs: https://parseforme.com/developers\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: A `pfm_live_…` workspace key\n  sources:\n  - openapi/parseforme-openapi-original.json\ndetails:\n  credential: \"workspace API key sent as Authorization: Bearer pfm_live_...\"\n  key_format: 'pfm_live_ + 43 base64url characters - 52 chars carrying 256 bits of entropy'\n  scanning_regex: '\\bpfm_live_[A-Za-z0-9_-]{43}\\b'\n  scanning_note: The shape is fixed and published so consumers can add it to their own secret scanning.\n  issuance: Created in the dashboard under Settings -> API keys by an owner or admin, shown once.\n  revocation: Revocable at any time; takes effect immediately.\n  limits: Up to 10 active keys per workspace.\n  scope: >-\n    A key acts as a member of one workspace - it can create, read and export\
  \ documents and manage webhook\n    endpoints; it can never manage members, billing or other keys. Keys work only on /v1/*.\n  failure_mode: >-\n    Every authentication failure returns the same opaque 401 whatever was wrong with the key - a response\n    distinguishing \"unknown\" from \"revoked\" would be a probing oracle.\n  note: >-\n    The OpenAPI's bearerFormat says JWT but the credential is an opaque pfm_live_ workspace key, not a\n    JWT - the docs are authoritative here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parseforme/refs/heads/main/authentication/parseforme-authentication.yml
summary_line: http · 1 scheme
tags:
- Document Parsing
- OCR
- Data Extraction
- Document AI
- IDP
- Invoices
- Bank Statements
- Receipts
- Resumes
- PDF
- Webhooks
- REST
---
