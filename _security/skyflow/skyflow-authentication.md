---
api_key_in: []
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Skyflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Skyflow secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Skyflow
provider_slug: skyflow
scheme_count: 2
schemes:
- applies_to:
  - Data API
  - Management API
  - SDKs
  bearer_format: JWT
  description: JWT bearer token (recommended). Time-limited (SDK-generated tokens are valid for 60 minutes). Generated from a service account's credentials.json via a Skyflow SDK, a Python script, or Skyflow Studio. Matches the RFC 6750 Authorization Bearer Token Header spec. Scoped by the roles/policies attached to the service account; supports context-aware authentication (context_identifier injected into the token).
  name: BearerToken
  scheme: bearer
  type: http
- applies_to:
  - Data API
  - Management API
  description: Long-lived API key, presented as a bearer credential in the Authorization header. Alternative to JWT bearer tokens; use only with a valid business need. Scoped by service-account roles/policies.
  in: header
  name: ApiKey
  parameter: Authorization
  type: apiKey
slug: skyflow-authentication
source_filename: skyflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.skyflow.com/docs/fundamentals/api-authentication\ndocs: https://docs.skyflow.com/docs/fundamentals/api-authentication\nsummary:\n  types: [http, apiKey]\n  http_schemes: [bearer]\n  bearer_format: JWT\n  standards: [RFC 6750]\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    JWT bearer token (recommended). Time-limited (SDK-generated tokens are\n    valid for 60 minutes). Generated from a service account's credentials.json\n    via a Skyflow SDK, a Python script, or Skyflow Studio. Matches the RFC 6750\n    Authorization Bearer Token Header spec. Scoped by the roles/policies\n    attached to the service account; supports context-aware authentication\n    (context_identifier injected into the token).\n  applies_to: [Data API, Management API, SDKs]\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    Long-lived\
  \ API key, presented as a bearer credential in the Authorization\n    header. Alternative to JWT bearer tokens; use only with a valid business\n    need. Scoped by service-account roles/policies.\n  applies_to: [Data API, Management API]\nidentity:\n  service_accounts: true\n  credentials_artifact: credentials.json\n  context_aware_auth: https://docs.skyflow.com/docs/governance/context-aware-auth/overview\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skyflow/refs/heads/main/authentication/skyflow-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Data Privacy
- PII
- Tokenization
- Data Security
- Vault
- Compliance
- PCI
- Encryption
- Data Governance
---
