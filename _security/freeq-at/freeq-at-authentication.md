---
anonymous_access: false
api_key_in: []
api_specs:
- filename: freeq-at-openapi.yml
  format: yaml
  label: freeq IRC API
  slug: freeq-irc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeq-at/openapi/freeq-at-openapi.yml
auth_types: []
description: Authentication schemes for freeq as documented
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: freeq Authentication
name_suffix: Authentication
oauth_flows: []
overview: freeq declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: freeq
provider_slug: freeq-at
scheme_count: 3
schemes:
- authorize_url: https://auth.freeq.at/auth/login
  evidence: 'OAuth token (web/iOS): Browser-based Bluesky login → broker mints a web-token'
  flows:
  - authorization_code
  how_to_obtain: User logs in via the Bluesky OAuth popup; the broker obtains a PDS token and mints a web‑token.
  name: OAuth token (web/iOS)
  type: oauth2
- evidence: App password (legacy)
  how_to_obtain: User generates an app password in Bluesky and passes it to the freeq‑tui client.
  name: App password (legacy)
  type: other
- evidence: 'Crypto key (bots): Direct ed25519/secp256k1 key → signs challenge directly'
  how_to_obtain: Bot provides its own ed25519 or secp256k1 private key which is used to sign the SASL challenge.
  name: Crypto key (bots)
  type: other
slug: freeq-at-authentication
source_filename: freeq-at-authentication.yml
source_heading: Authentication Profile
source_url: https://freeq.at/docs/authentication.md
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://freeq.at/docs/authentication.md\nsources:\n- https://freeq.at/docs/authentication.md\n- https://freeq.at/docs/authentication/\n- https://freeq.at/docs/getting-started.md\n- https://freeq.at/docs/agent-quickstart.md\ndescription: Authentication schemes for freeq as documented\nschemes:\n- type: oauth2\n  name: OAuth token (web/iOS)\n  evidence: 'OAuth token (web/iOS): Browser-based Bluesky login → broker mints a web-token'\n  flows:\n  - authorization_code\n  authorize_url: https://auth.freeq.at/auth/login\n  how_to_obtain: User logs in via the Bluesky OAuth popup; the broker obtains a PDS token and mints a web‑token.\n- type: other\n  name: App password (legacy)\n  evidence: App password (legacy)\n  how_to_obtain: User generates an app password in Bluesky and passes it to the freeq‑tui client.\n- type: other\n  name: Crypto key (bots)\n  evidence: 'Crypto key (bots): Direct\
  \ ed25519/secp256k1 key → signs challenge directly'\n  how_to_obtain: Bot provides its own ed25519 or secp256k1 private key which is used to sign the SASL challenge.\ndocs: https://freeq.at/docs/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/freeq-at/authentication/freeq-at-authentication.yml
summary_line: 3 schemes
tags:
- Chat
- Identity
- Encryption
- Open Source
- Irc
---
