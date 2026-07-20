---
api_key_in: []
auth_types:
- http-bearer
- service-account
description: ''
kind: authentication
layout: security
method: searched
name: Ascendio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ascend.io secures its APIs with http-bearer and service-account across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ascend.io
provider_slug: ascendio
scheme_count: 1
schemes:
- credential: Ed25519 service account key (asc-sa-...)
  header: 'Authorization: Bearer <token>'
  name: serviceAccountBearer
  note: Token obtained via Ed25519 JWT assertion -> Cloud API token exchange; cached with refresh mutex.
  scheme: bearer
  token_endpoint_family: /api/v1/auth/*
  type: http
slug: ascendio-authentication
source_filename: ascendio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.ascend.io/getting-started/quickstart + https://github.com/ascend-io/ascend-tools (AGENTS.md, crates/ascend-tools-core/src/auth.rs)\ndocs: https://docs.ascend.io\nsummary:\n  types: [http-bearer, service-account]\n  api_key_in: []\n  token_exchange: true\nmodel: >-\n  The Ascend Instance web API uses service-account authentication. A service account (id\n  prefix `asc-sa-...`) is created in the Ascend UI (Settings > Users > Create Service Account)\n  and issued an Ed25519 private key (base64url, shown once at creation). The SDK/CLI signs an\n  Ed25519 JWT assertion and exchanges it via the Cloud API token-exchange flow for a short-lived\n  Bearer token, which is cached and attached as `Authorization: Bearer <token>` on every\n  `/api/v1/*` request (except `/api/v1/auth/*`).\nschemes:\n  - name: serviceAccountBearer\n    type: http\n    scheme: bearer\n    credential: Ed25519 service account key (asc-sa-...)\n  \
  \  header: 'Authorization: Bearer <token>'\n    token_endpoint_family: /api/v1/auth/*\n    note: Token obtained via Ed25519 JWT assertion -> Cloud API token exchange; cached with refresh mutex.\ncredentials:\n  env:\n    - name: ASCEND_SERVICE_ACCOUNT_ID\n      description: Service account ID (asc-sa-...)\n    - name: ASCEND_SERVICE_ACCOUNT_KEY\n      description: Ed25519 private key (base64url, shown once at creation)\n    - name: ASCEND_INSTANCE_API_URL\n      description: Instance API URL (e.g. https://api.instance.ascend.io)\n  config_file: ~/.ascend-tools/config.toml\n  resolution_order: [cli-flags, instance-config-toml, env-vars]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ascendio/refs/heads/main/authentication/ascendio-authentication.yml
summary_line: http-bearer/service-account · 1 scheme
tags:
- Company
- Big Data
- Data Engineering
- Data Pipelines
- ETL
- Orchestration
- Data Automation
- MCP
- Developer Tools
---
