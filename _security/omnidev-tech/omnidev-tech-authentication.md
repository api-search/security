---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for OmniDev Tech API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Omnidev Tech Authentication
name_suffix: Authentication
oauth_flows: []
overview: omnidev-tech declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: omnidev-tech
provider_slug: omnidev-tech
scheme_count: 2
schemes:
- evidence: 'Authorization: Bearer $OMNI_API_KEY'
  header: Authorization
  how_to_obtain: Obtain an API key after completing a package checkout; the success page returns your API key.
  location: header
  name: Authorization
  type: http-bearer
- evidence: 'Call POST https://pay.omnidev.tech/v1/chat/completions with wallet-signed headers X-Omni-Wallet , X-Omni-Wallet-Ts , X-Omni-Wallet-Sig (an EIP-191 signature over: host, METHOD path, timestamp, body hash).'
  header: X-Omni-Wallet, X-Omni-Wallet-Ts, X-Omni-Wallet-Sig
  how_to_obtain: Create a wallet that can sign EIP‑191 requests; the paying address owns the balance.
  location: header
  name: wallet
  type: other
slug: omnidev-tech-authentication
source_filename: omnidev-tech-authentication.yml
source_heading: Authentication Profile
source_url: https://pay.omnidev.tech/v1/bundles
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://pay.omnidev.tech/v1/bundles\nsources:\n- https://pay.omnidev.tech/v1/bundles\n- https://provider.omnidev.tech/docs/bundles\n- https://provider.omnidev.tech/docs/quickstart\ndescription: Authentication schemes for OmniDev Tech API\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Authorization: Bearer $OMNI_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain an API key after completing a package checkout; the success page returns your API key.\n- type: other\n  name: wallet\n  evidence: 'Call POST https://pay.omnidev.tech/v1/chat/completions with wallet-signed headers X-Omni-Wallet , X-Omni-Wallet-Ts , X-Omni-Wallet-Sig\n    (an EIP-191 signature over: host, METHOD path, timestamp, body hash).'\n  location: header\n  header: X-Omni-Wallet, X-Omni-Wallet-Ts, X-Omni-Wallet-Sig\n  how_to_obtain: Create a wallet that can sign EIP‑191\
  \ requests; the paying address owns the balance.\ndocs: https://pay.omnidev.tech/v1/bundles\n"
source_yaml_url: https://artifacts.apis.io/omnidev-tech/authentication/omnidev-tech-authentication.yml
summary_line: 2 schemes
tags:
- AI
- LLM
- Pay-per-call
- Developer-friendly
- Company
---
