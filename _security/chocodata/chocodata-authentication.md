---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: chocodata-openapi.json
  format: json
  label: Chocodata Scraper API
  slug: chocodata-scraper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chocodata/refs/heads/main/openapi/chocodata-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Chocodata Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chocodata secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chocodata
provider_slug: chocodata
scheme_count: 1
schemes:
- detail: The api_key query parameter is the ONLY accepted auth location — Authorization Bearer and X-API-Key headers both return 401. Unauthorized requests are free (never billed).
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/chocodata-openapi.json
  - https://chocodata.com/docs/guides/authentication
  type: apiKey
slug: chocodata-authentication
source_filename: chocodata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: https://chocodata.com/docs/guides/authentication\ndocs: https://chocodata.com/docs/guides/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/chocodata-openapi.json\n  - https://chocodata.com/docs/guides/authentication\n  detail: >-\n    The api_key query parameter is the ONLY accepted auth location — Authorization Bearer and\n    X-API-Key headers both return 401. Unauthorized requests are free (never billed).\nkey_management:\n  prefixes:\n    - prefix: asa_live_\n      meaning: Production keys\n    - prefix: cd_test_\n      meaning: Sandbox keys (roadmap — not shipped; would return deterministic fixtures without billing)\n  shortprefix: The 12 characters after the prefix identify a key in the dashboard and logs without revealing the secret.\n  issuance: Sign up at https://app.chocodata.com (Google\
  \ or email+password, no card for free tier); Settings > API keys > Generate new key; full key shown exactly once.\n  rotation: Generate a second key, deploy, revoke the old; revocation is global within ~30 seconds and returns 401 {\"error\":\"revoked\"}.\n  limits: Up to 20 active keys per workspace; plan credit allowance is per workspace, aggregated across keys; per-key usage filtering in the dashboard.\n  ip_allowlists: Roadmap feature for Pro and Custom plans (manual enablement via info@chocodata.com).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chocodata/refs/heads/main/authentication/chocodata-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web Scraping
- Data Extraction
- SERP
- E-Commerce Data
- social-media-data
- Proxy
- MCP
- agent-native
- structured-json
---
