---
api_key_in: []
api_specs:
- filename: zyte-zyte-api-openapi.yaml
  format: yaml
  label: Zyte API
  slug: zyte
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zyte/refs/heads/main/openapi/zyte-zyte-api-openapi.yaml
- filename: zyte-stats-api-openapi.yaml
  format: yaml
  label: Zyte API Stats API
  slug: zyte-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zyte/refs/heads/main/openapi/zyte-stats-api-openapi.yaml
auth_types:
- http
description: Every Zyte HTTP surface uses the same mechanism — RFC 7617 HTTP Basic with the API key as username and an EMPTY password — but they do NOT share the same key. Zyte runs three separate key namespaces, and the docs call this out explicitly ("Scrapy Cloud uses a different API key than Zyte API"; the Stats API needs "your Zyte dashboard API key (not your Zyte API key)"). An agent holding one Zyte key can call exactly one of the three surfaces. There are no OAuth flows, no scopes, and no token exchange anywhere in the estate, so scopes/ is intentionally absent for this provider.
kind: authentication
layout: security
method: searched
name: Zyte Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zyte secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zyte
provider_slug: zyte
scheme_count: 1
schemes:
- applied_to: all operations in both specs
  format: Basic base64("<API_KEY>:")
  header: Authorization
  in: header
  name: BasicAuth
  password: empty
  scheme: basic
  sources:
  - openapi/zyte-zyte-api-openapi.yaml
  - openapi/zyte-stats-api-openapi.yaml
  type: http
slug: zyte-authentication
source_filename: zyte-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: >-\n  https://docs.zyte.com/zyte-api/usage/reference.html,\n  https://docs.zyte.com/zyte-api/usage/stats/index.html,\n  https://docs.zyte.com/scrapy-cloud/usage/reference/http/index.html,\n  https://python-zyte-api.readthedocs.io/en/stable/ref/cli.html\ndocs: https://docs.zyte.com/zyte-api/get-started.html\nprovider: Zyte\nproviderId: zyte\nsummary:\n  types:\n    - http\n  schemes: 1\n  oauth2: false\n  scopes: false\ndescription: >-\n  Every Zyte HTTP surface uses the same mechanism — RFC 7617 HTTP Basic with the\n  API key as username and an EMPTY password — but they do NOT share the same\n  key. Zyte runs three separate key namespaces, and the docs call this out\n  explicitly (\"Scrapy Cloud uses a different API key than Zyte API\"; the Stats\n  API needs \"your Zyte dashboard API key (not your Zyte API key)\"). An agent\n  holding one Zyte key can call exactly one of the three surfaces. There are no\n  OAuth flows, no\
  \ scopes, and no token exchange anywhere in the estate, so\n  scopes/ is intentionally absent for this provider.\nschemes:\n  - name: BasicAuth\n    type: http\n    scheme: basic\n    in: header\n    header: Authorization\n    format: 'Basic base64(\"<API_KEY>:\")'\n    password: empty\n    sources:\n      - openapi/zyte-zyte-api-openapi.yaml\n      - openapi/zyte-stats-api-openapi.yaml\n    applied_to: all operations in both specs\nkey_namespaces:\n  - surface: Zyte API\n    host: https://api.zyte.com/v1\n    credential: Zyte API key\n    obtain: https://app.zyte.com/o/zyte-api/api-access\n    env_var: ZYTE_API_KEY\n    note: >-\n      Used by python-zyte-api, the zyte-api CLI and scrapy-zyte-api. Failure\n      modes are /auth/not-valid (401, malformed/missing) and /auth/key-not-found\n      (401, wrong key) — see errors/zyte-problem-types.yml.\n  - surface: Zyte API Stats API\n    host: https://zyte-api-stats.zyte.com\n    credential: Zyte dashboard API key\n    obtain: https://app.zyte.com/o/settings\n\
  \    note: >-\n      Documented explicitly as NOT the Zyte API key. Requests also require an\n      `organization_id` query parameter, which is the real tenancy boundary on\n      this surface.\n  - surface: Scrapy Cloud API\n    hosts:\n      - https://app.zyte.com/api\n      - https://storage.zyte.com\n    credential: Scrapy Cloud API key\n    obtain: https://app.zyte.com/o/settings/apikey\n    alternate_transport: >-\n      Also accepted as an `?apikey=` URL query parameter. This is a documented\n      convenience that puts a long-lived credential into URLs, request logs and\n      proxy history — prefer the Basic header.\n  - surface: Zyte API via x402\n    host: https://api.zyte.com/v1\n    credential: Ethereum private key (x402 machine payment protocol)\n    obtain: 'pip install \"zyte-api[x402]\"; zyte-api --eth-key ...'\n    note: >-\n      An alternative to holding a Zyte account key at all — the zyte-api CLI\n      accepts --eth-key (mutually exclusive with --api-key) and pays\
  \ per request\n      over x402. Genuinely notable: an agent can call Zyte API without ever\n      being onboarded as a Zyte customer.\n    source: https://python-zyte-api.readthedocs.io/en/stable/ref/cli.html\naccount_lifecycle:\n  suspension:\n    trigger:\n      - Trial free credit exhausted\n      - Monthly spending limit reached\n    response: '403 /auth/account-suspended'\n    recovery: >-\n      Setting or raising the spending limit lifts the suspension immediately.\n      Documented at https://docs.zyte.com/zyte-api/pricing.html#zapi-account-suspension\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zyte/refs/heads/main/authentication/zyte-authentication.yml
summary_line: http · 1 scheme
tags:
- Crawling
- Data Extraction
- Scraping
- Web Scraping
- Proxies
- Browser Automation
- Anti-Ban
- SERP
- Agent Skills
- Developer Tools
---
