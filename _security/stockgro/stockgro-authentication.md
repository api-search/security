---
api_key_in: []
api_specs:
- filename: stockgro-tradeview-intraday-model-openapi.json
  format: json
  label: TradeView Intraday Model API
  slug: stockgro-tradeview-intraday-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stockgro/refs/heads/main/openapi/stockgro-tradeview-intraday-model-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Stockgro Authentication
name_suffix: Authentication
oauth_flows: []
overview: StockGro declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: StockGro
provider_slug: stockgro
scheme_count: 0
schemes: []
slug: stockgro-authentication
source_filename: stockgro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: derived\nsource: openapi/stockgro-tradeview-intraday-model-openapi.json + live probes of api.stockgro.club\napi: stockgro-tradeview-intraday-model-api\nsummary: >-\n  The published OpenAPI declares NO components.securitySchemes and applies no security\n  requirement to any of its three operations. All three documented operations answered\n  anonymously on a live probe, so the documented surface is effectively unauthenticated.\n  StockGro publishes no developer authentication documentation, no API keys, and no\n  OAuth surface — this is an internal platform service, not a keyed developer API.\nschemes: []\nscheme_count: 0\napplied_globally: false\nobserved:\n- path: /\n  method: get\n  anonymous_status: 200\n  note: returned {\"message\":\"Trade Processing API is running\",\"environment\":\"prod\"}\n- path: /health\n  method: get\n  anonymous_status: 200\n  note: returned service health for kafka and clickhouse\n- path: /api-docs\n  method: get\n\
  \  anonymous_status: 401\n  note: >-\n    Not an operation in the published spec. A sibling path on the same host answered\n    401 \"Missing authorization token\", showing SOME token-based gate exists elsewhere on\n    api.stockgro.club; its scheme is not documented anywhere public and was not probed\n    further.\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_keys: false\ndocs: null\ndocs_note: >-\n  No public authentication documentation exists. api.stockgro.club/docs and /redoc are\n  the FastAPI-generated Swagger UI and ReDoc renderings of the same spec and contain no\n  auth guidance.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stockgro/refs/heads/main/authentication/stockgro-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Financial-Services
- Stock Market
- Investing
- Market Data
- Financial Education
- Fintech
- India
- Advisory
- Social Investing
---
