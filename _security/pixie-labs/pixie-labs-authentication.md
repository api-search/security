---
api_key_in:
- metadata
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Pixie Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pixie Labs secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Pixie Labs
provider_slug: pixie-labs
scheme_count: 2
schemes:
- description: Opaque API key (prefix px-api-) created with `px api-key create` or in the Live UI Admin > API Keys tab. Passed to the client library at construction (Go pxapi.WithAPIKey(...), Python pxapi.Client(token=...)) and sent on the gRPC connection to Pixie Cloud/Vizier. A Cluster ID identifies the target cluster.
  docs: https://docs.px.dev/reference/admin/api-keys/
  in: metadata
  key_prefix: px-api-
  name: PixieApiKey
  type: apiKey
- description: Deploy keys (`px deploy-key`) are a distinct credential used when deploying Pixie (Vizier) to register a new cluster with Pixie Cloud; not used for API script execution.
  docs: https://docs.px.dev/reference/admin/deploy-keys/
  in: metadata
  name: PixieDeployKey
  type: apiKey
slug: pixie-labs-authentication
source_filename: pixie-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.px.dev/reference/admin/api-keys/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - metadata\n  oauth2_flows: []\n  note: >-\n    Pixie has no OpenAPI (gRPC-only API), so this profile is captured from the\n    provider docs rather than derived from a spec.\nschemes:\n- name: PixieApiKey\n  type: apiKey\n  in: metadata\n  description: >-\n    Opaque API key (prefix px-api-) created with `px api-key create` or in the\n    Live UI Admin > API Keys tab. Passed to the client library at construction\n    (Go pxapi.WithAPIKey(...), Python pxapi.Client(token=...)) and sent on the\n    gRPC connection to Pixie Cloud/Vizier. A Cluster ID identifies the target\n    cluster.\n  key_prefix: px-api-\n  docs: https://docs.px.dev/reference/admin/api-keys/\n- name: PixieDeployKey\n  type: apiKey\n  in: metadata\n  description: >-\n    Deploy keys (`px deploy-key`) are a distinct credential used when deploying\n    Pixie (Vizier)\
  \ to register a new cluster with Pixie Cloud; not used for API\n    script execution.\n  docs: https://docs.px.dev/reference/admin/deploy-keys/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixie-labs/refs/heads/main/authentication/pixie-labs-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Ai
- Observability
- Kubernetes
- eBPF
- Monitoring
- Tracing
- Open Source
- CNCF
- gRPC
- Developer Tools
---
