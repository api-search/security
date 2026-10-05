---
anonymous_access: true
api_key_in: []
api_specs:
- filename: quietforge-convert-api-openapi.yml
  format: yaml
  label: Quietforge Document Conversion API
  slug: document-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quietforge/refs/heads/main/openapi/quietforge-convert-api-openapi.yml
- filename: quietforge-x402-index-api-openapi.yml
  format: yaml
  label: Quietforge x402 Service Index API
  slug: x402-service-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quietforge/refs/heads/main/openapi/quietforge-x402-index-api-openapi.yml
- filename: quietforge-sudoku-api-openapi.yml
  format: yaml
  label: Quietforge Puzzle Generation API
  slug: puzzle-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quietforge/refs/heads/main/openapi/quietforge-sudoku-api-openapi.yml
- filename: quietforge-typeset-api-openapi.yml
  format: yaml
  label: Quietforge Book Typesetting API
  slug: book-typesetting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quietforge/refs/heads/main/openapi/quietforge-typeset-api-openapi.yml
- filename: quietforge-familytree-api-openapi.yml
  format: yaml
  label: Quietforge Family Tree Chart API
  slug: family-chart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quietforge/refs/heads/main/openapi/quietforge-familytree-api-openapi.yml
- filename: quietforge-dataset-audit-api-openapi.yml
  format: yaml
  label: Quietforge Dataset Audit API
  slug: dataset-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quietforge/refs/heads/main/openapi/quietforge-dataset-audit-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Quietforge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quietforge Studio declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Quietforge Studio
provider_slug: quietforge
scheme_count: 2
schemes:
- applies_to:
  - https://qf-api.quietforge-studio.workers.dev/v1/*
  evidence: 'Live 2026-10-03: GET /v1/x402/services and POST /v1/sudoku without payment returned 402 with a payment-required header (x402Version 2); a nonsense path returned 404. The OpenAPI declares no securitySchemes; prices are in each operation x-payment-info.'
  name: x402
  type: payment
- applies_to:
  - https://qf-api.quietforge-studio.workers.dev/mcp
  - https://qf-api.quietforge-studio.workers.dev/v1/samples
  - https://qf-api.quietforge-studio.workers.dev/v1/dataset-audit/preview
  evidence: MCP initialize + tools/list succeeded with no credentials on 2026-10-03.
  name: anonymous
  type: none
slug: quietforge-authentication
source_filename: quietforge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource:\n- https://qf-api.quietforge-studio.workers.dev/.well-known/x402\n- https://qf-api.quietforge-studio.workers.dev/openapi.json\nsummary: No API key, account, OAuth or bearer token. Paid routes answer an unpaid request with HTTP 402 and a PAYMENT-REQUIRED\n  header (x402 v2); the caller pays per request in USDC on Base (eip155:8453) and retries. Free routes (GET /health, GET /.well-known/x402,\n  POST /v1/dataset-audit/preview, GET /v1/samples) and the MCP server need nothing.\nrequires_auth: true\npublic: true\nschemes:\n- name: x402\n  type: payment\n  applies_to:\n  - https://qf-api.quietforge-studio.workers.dev/v1/*\n  evidence: 'Live 2026-10-03: GET /v1/x402/services and POST /v1/sudoku without payment returned 402 with a payment-required\n    header (x402Version 2); a nonsense path returned 404. The OpenAPI declares no securitySchemes; prices are in each operation\n    x-payment-info.'\n- name: anonymous\n  type: none\n \
  \ applies_to:\n  - https://qf-api.quietforge-studio.workers.dev/mcp\n  - https://qf-api.quietforge-studio.workers.dev/v1/samples\n  - https://qf-api.quietforge-studio.workers.dev/v1/dataset-audit/preview\n  evidence: MCP initialize + tools/list succeeded with no credentials on 2026-10-03.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quietforge/refs/heads/main/authentication/quietforge-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Document Processing
- x402
- Micropayments
- MCP
- pay-per-call
- Cloudflare Workers
- Software-as-a-Service
- Business Automation
---
