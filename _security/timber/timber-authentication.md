---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Timber Authentication
name_suffix: Authentication
oauth_flows: []
overview: Timber secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Timber
provider_slug: timber
scheme_count: 0
schemes: []
slug: timber-authentication
source_filename: timber-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://vector.dev/docs/reference/api/\napi: Vector Observability API\nsummary:\n  types: [none]\n  authenticated: false\n  note: >-\n    The Vector Observability API (gRPC, plus a GET /health HTTP endpoint on the\n    same port) does not support authentication. The documentation explicitly\n    warns that it must only be enabled in isolated environments or for debugging\n    and must not be exposed to untrusted clients. There is no OAuth, API key, or\n    bearer-token surface. Access control is expected to be handled at the network\n    layer (bind address / firewall) rather than in the API itself.\nschemes: []\nnetwork_controls:\n  - control: bind-address\n    default: 127.0.0.1:8686\n    description: >-\n      The API binds to loopback by default (api.address). To expose it (e.g. in a\n      Docker container) it must be bound to 0.0.0.0, which the docs flag as a\n      security-sensitive change to guard at the network level.\n\
  \  - control: enablement-flag\n    field: api.enabled\n    default: false\n    description: The API is disabled by default and must be explicitly enabled.\ndocs:\n  - https://vector.dev/docs/reference/api/\n  - https://vector.dev/docs/reference/configuration/global-options/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/timber/refs/heads/main/authentication/timber-authentication.yml
summary_line: none · 0 schemes
tags:
- Company
- Developer Tools
- Observability
- Logs
- Metrics
- Data Pipeline
- Logging
- Monitoring
- Open Source
- gRPC
- Rust
- Datadog
---
