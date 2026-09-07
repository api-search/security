---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: openapi.json
  format: json
  label: Offendersearch API
  slug: offendersearch-api
  spec_type: OpenAPI
  url: https://offendersearch.app/openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Offendersearch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Offendersearch secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Offendersearch
provider_slug: offendersearch
scheme_count: 4
schemes:
- description: Customer API key. Primary auth for search/records/compat/proof.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/offendersearch-openapi.json
  - openapi/offendersearch-openapi.yaml
  type: apiKey
- description: Signed session token (HMAC-SHA256). Auth for account/dashboard endpoints; also accepted by POST /v1/search and the compat endpoint.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/offendersearch-openapi.json
  - openapi/offendersearch-openapi.yaml
  type: http
- description: API key passed as `?key=` — offenders.io demo mode (compat endpoint only).
  in: query
  name: QueryKeyAuth
  parameter: key
  sources:
  - openapi/offendersearch-openapi.json
  - openapi/offendersearch-openapi.yaml
  type: apiKey
- description: Internal admin credential — separate from customer API keys.
  in: header
  name: AdminAuth
  parameter: X-Admin-Key
  sources:
  - openapi/offendersearch-openapi.json
  - openapi/offendersearch-openapi.yaml
  type: apiKey
slug: offendersearch-authentication
source_filename: offendersearch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: openapi/offendersearch-openapi.json + https://offendersearch.app/docs/authentication.md\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Customer API key. Primary auth for search/records/compat/proof.\n  sources:\n  - openapi/offendersearch-openapi.json\n  - openapi/offendersearch-openapi.yaml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Signed session token (HMAC-SHA256). Auth for account/dashboard endpoints; also accepted\n    by POST /v1/search and the compat endpoint.\n  sources:\n  - openapi/offendersearch-openapi.json\n  - openapi/offendersearch-openapi.yaml\n- name: QueryKeyAuth\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key passed as `?key=` — offenders.io demo mode (compat endpoint only).\n  sources:\n  - openapi/offendersearch-openapi.json\n\
  \  - openapi/offendersearch-openapi.yaml\n- name: AdminAuth\n  type: apiKey\n  in: header\n  parameter: X-Admin-Key\n  description: Internal admin credential — separate from customer API keys.\n  sources:\n  - openapi/offendersearch-openapi.json\n  - openapi/offendersearch-openapi.yaml\ndocs: https://offendersearch.app/docs/authentication.md\nkey_lifecycle:\n  prefix: os_live_\n  creation: Keys are created, named, rotated and revoked from the dashboard/API keys page; the secret\n    is shown in full only once, at creation, and stored only as a one-way hash.\n  rotation: Issue a second key, deploy it, then revoke the first — both valid at once, so rotation needs\n    no downtime window.\n  scoping: A key is a pure authentication credential — no per-key feature scopes; every key can call every\n    documented endpoint. Usage is attributed per key.\nsecurity_posture:\n  encryption: TLS in transit, AES-256 at rest for stored records and reports\n  tenant_isolation: Data scoped per account;\
  \ audit logging of account, timestamp and endpoint\n  baa: Business Associate Agreement available to eligible enterprise accounts (HIPAA-ready path)\n  source: https://offendersearch.app/docs/authentication.md\nnotes: AdminAuth (X-Admin-Key) is an internal credential, not part of the public API; QueryKeyAuth (?key=)\n  exists only for the offenders.io compat endpoint demo mode.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/offendersearch/refs/heads/main/authentication/offendersearch-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Background Screening
- Identity & risk
- Trust and Safety
- Public Records
- Criminal data
- Compliance
- Sex-offender registry data
- Staffing & recruiting
- Tenant Screening
- Healthcare
- Gig marketplaces
---
