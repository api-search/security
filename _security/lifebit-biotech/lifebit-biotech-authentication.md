---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lifebit Biotech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lifebit Biotech secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lifebit Biotech
provider_slug: lifebit-biotech
scheme_count: 2
schemes:
- description: The primary CloudOS API credential. A workspace API key is issued from the Lifebit Platform UI and sent on every request as an `apikey` header. The CLI accepts it via --apikey or reads it from a named profile in ~/.cloudos/credentials.
  in: header
  name: apikey
  parameter_name: apikey
  scope_model: Keys are workspace-scoped rather than scope-scoped. Requests additionally carry a teamId query parameter identifying the workspace, and the API rejects cross-workspace access. There is no OAuth scope surface.
  sources:
  - https://github.com/lifebit-ai/cloudos-cli/blob/main/cloudos_cli/clos.py
  type: apiKey
- description: 'A separate bearer token used only for the Cromwell/WDL subsystem, sent as `Authorization: Bearer <token>` when driving the Cromwell server endpoints under /api/v1/cromwell.'
  name: cromwell_token
  scheme: bearer
  sources:
  - https://github.com/lifebit-ai/cloudos-cli/blob/main/cloudos_cli/clos.py
  type: http
slug: lifebit-biotech-authentication
source_filename: lifebit-biotech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: https://github.com/lifebit-ai/cloudos-cli\ndocs: https://lifebit-ai.github.io/cloudos-cli/getting_started.html\nnotes: >-\n  Lifebit publishes no OpenAPI description for the CloudOS API, so the\n  derive-authentication.py pass had no spec to read. This profile is derived\n  from the first-party open-source client (cloudos-cli): the request headers it\n  sets, the credential handling in cloudos_cli/configure, and the\n  authorisation errors it raises. Verified live: an unauthenticated GET to\n  https://cloudos.lifebit.ai/api/v1/users/me returns HTTP 401.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: apikey\n  type: apiKey\n  in: header\n  parameter_name: apikey\n  description: >-\n    The primary CloudOS API credential. A workspace API key is issued from the\n    Lifebit Platform UI and sent on every request\
  \ as an `apikey` header. The CLI\n    accepts it via --apikey or reads it from a named profile in\n    ~/.cloudos/credentials.\n  scope_model: >-\n    Keys are workspace-scoped rather than scope-scoped. Requests additionally\n    carry a teamId query parameter identifying the workspace, and the API\n    rejects cross-workspace access. There is no OAuth scope surface.\n  sources:\n  - https://github.com/lifebit-ai/cloudos-cli/blob/main/cloudos_cli/clos.py\n- name: cromwell_token\n  type: http\n  scheme: bearer\n  description: >-\n    A separate bearer token used only for the Cromwell/WDL subsystem, sent as\n    `Authorization: Bearer <token>` when driving the Cromwell server endpoints\n    under /api/v1/cromwell.\n  sources:\n  - https://github.com/lifebit-ai/cloudos-cli/blob/main/cloudos_cli/clos.py\ncredential_storage:\n  file: ~/.cloudos/credentials\n  managed_by: cloudos configure\n  supports_named_profiles: true\nauthorization_errors:\n- status: 401\n  meaning: Missing or invalid apikey.\n\
  - status: 403\n  meaning: >-\n    Authenticated but not permitted — the requested resource is outside the\n    workspace named by teamId, or the job belongs to another user.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lifebit-biotech/refs/heads/main/authentication/lifebit-biotech-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Health
- Genomics
- Bioinformatics
- Federated Learning
- Trusted Research Environment
- Data Governance
- Life Sciences
- Sovereign AI
- OMOP
- Workflow Orchestration
---
