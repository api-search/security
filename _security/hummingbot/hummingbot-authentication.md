---
api_key_in: []
api_specs:
- filename: hummingbot-gateway-openapi-original.json
  format: json
  label: Hummingbot Gateway
  slug: hummingbot-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingbot/refs/heads/main/openapi/hummingbot-gateway-openapi-original.json
auth_types:
- http-basic
- passphrase
- mtls-optional
description: 'Hummingbot''s two server components authenticate differently, and neither uses OAuth or issued API tokens: the Hummingbot API uses HTTP Basic auth, while Gateway protects wallet keys with a startup passphrase and TLS.'
kind: authentication
layout: security
method: searched
name: Hummingbot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hummingbot secures its APIs with http-basic, passphrase, and mtls-optional across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hummingbot
provider_slug: hummingbot
scheme_count: 3
schemes:
- component: Hummingbot API (FastAPI server, default :8000)
  detail: Username/password set during `make setup` (defaults admin/admin, meant to be changed). Sent as an HTTP Basic Authorization header on every request.
  docs: https://hummingbot.org/hummingbot-api/
  name: HummingbotAPIBasic
  scheme: basic
  type: http
- component: Gateway (TypeScript DEX middleware, default :15888)
  detail: Gateway is started with `--passphrase=<PASSPHRASE>`; the passphrase encrypts the wallet key store. There is no per-request API token — access control is network isolation plus the encrypted wallet. Production mode requires TLS certificates (HTTPS); `--dev` runs unencrypted HTTP for local use.
  docs: https://hummingbot.org/gateway/
  name: GatewayPassphrase
  type: passphrase
- component: Gateway (production mode)
  detail: In production Gateway serves HTTPS with TLS certificates; client certs can be used to restrict access to the Gateway host.
  docs: https://hummingbot.org/gateway/
  name: GatewayTLS
  optional: true
  type: mutualTLS
slug: hummingbot-authentication
source_filename: hummingbot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://hummingbot.org/hummingbot-api/, https://github.com/hummingbot/hummingbot-api,\n  https://github.com/hummingbot/gateway — auth captured from the component docs\n  and READMEs. The Gateway OpenAPI declares no securitySchemes, so this profile\n  is documentation-sourced rather than spec-derived.\ndescription: >-\n  Hummingbot's two server components authenticate differently, and neither uses\n  OAuth or issued API tokens: the Hummingbot API uses HTTP Basic auth, while\n  Gateway protects wallet keys with a startup passphrase and TLS.\nsummary:\n  types: [http-basic, passphrase, mtls-optional]\n  hosted_oauth: false\n  api_keys: false\nschemes:\n  - name: HummingbotAPIBasic\n    component: Hummingbot API (FastAPI server, default :8000)\n    type: http\n    scheme: basic\n    detail: >-\n      Username/password set during `make setup` (defaults admin/admin, meant to\n      be changed). Sent as an HTTP Basic Authorization\
  \ header on every request.\n    docs: https://hummingbot.org/hummingbot-api/\n  - name: GatewayPassphrase\n    component: Gateway (TypeScript DEX middleware, default :15888)\n    type: passphrase\n    detail: >-\n      Gateway is started with `--passphrase=<PASSPHRASE>`; the passphrase encrypts\n      the wallet key store. There is no per-request API token — access control is\n      network isolation plus the encrypted wallet. Production mode requires TLS\n      certificates (HTTPS); `--dev` runs unencrypted HTTP for local use.\n    docs: https://hummingbot.org/gateway/\n  - name: GatewayTLS\n    component: Gateway (production mode)\n    type: mutualTLS\n    optional: true\n    detail: >-\n      In production Gateway serves HTTPS with TLS certificates; client certs can\n      be used to restrict access to the Gateway host.\n    docs: https://hummingbot.org/gateway/\nexchange_credentials:\n  note: >-\n    Individual CEX/DEX connectors require the user's own exchange API keys\n    (entered\
  \ via the Hummingbot client `connect` command or stored per-account\n    via the API `add_credential`). These are the end user's exchange keys, not a\n    Hummingbot-issued credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hummingbot/refs/heads/main/authentication/hummingbot-authentication.yml
summary_line: http-basic/passphrase/mtls-optional · 3 schemes
tags:
- Company
- Crypto
- Trading
- Blockchain
- DeFi
- DEX
- Open Source
- Market Making
- Algorithmic Trading
- Bots
---
