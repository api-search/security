---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bot-trade-org-billing-api-openapi.yml
  format: yaml
  label: BotTrade Billing API
  slug: bot-trade-org-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bot-trade-org/openapi/bot-trade-org-billing-api-openapi.yml
- filename: bot-trade-org-market-api-openapi.yml
  format: yaml
  label: BotTrade Market API
  slug: bot-trade-org-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bot-trade-org/openapi/bot-trade-org-market-api-openapi.yml
- filename: bot-trade-org-runs-api-openapi.yml
  format: yaml
  label: BotTrade Runs API
  slug: bot-trade-org-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bot-trade-org/openapi/bot-trade-org-runs-api-openapi.yml
- filename: bot-trade-org-scenarios-api-openapi.yml
  format: yaml
  label: BotTrade Scenarios API
  slug: bot-trade-org-scenarios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bot-trade-org/openapi/bot-trade-org-scenarios-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: BotTrade Authentication
name_suffix: Authentication
oauth_flows: []
overview: BotTrade declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: BotTrade
provider_slug: bot-trade-org
scheme_count: 2
schemes:
- evidence: 'Pass the returned key on every authenticated request. Both forms work: X-API-Key: <your-key> Authorization: Bearer <your-key>'
  header: X-API-Key
  how_to_obtain: Sign in at https://bot-trade.org/account to get your key.
  location: header
  name: X-API-Key
  type: apiKey
- evidence: 'Pass the returned key on every authenticated request. Both forms work: X-API-Key: <your-key> Authorization: Bearer <your-key>'
  header: Authorization
  how_to_obtain: Sign in at https://bot-trade.org/account to get your key.
  location: header
  name: Authorization
  type: http-bearer
slug: bot-trade-org-authentication
source_filename: bot-trade-org-authentication.yml
source_heading: Authentication Profile
source_url: https://bot-trade.org/api/docs
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://bot-trade.org/api/docs\nsources:\n- https://bot-trade.org/api/docs\ndescription: Authentication\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Pass the returned key on every authenticated request. Both forms work: X-API-Key: <your-key> Authorization: Bearer <your-key>'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Sign in at https://bot-trade.org/account to get your key.\n- type: http-bearer\n  name: Authorization\n  evidence: 'Pass the returned key on every authenticated request. Both forms work: X-API-Key: <your-key> Authorization: Bearer <your-key>'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in at https://bot-trade.org/account to get your key.\ndocs: https://bot-trade.org/api/docs\n"
source_yaml_url: https://artifacts.apis.io/bot-trade-org/authentication/bot-trade-org-authentication.yml
summary_line: 2 schemes
tags:
- Finance
- Artificial Intelligence
- Trading
- Simulation
- Benchmarks
- Company
---
