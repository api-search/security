---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication is performed by obtaining a short‑lived 8‑character code from the Telegram bot @barryauthbot and submitting it on the login page.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Tachyo Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: tachyo-ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: tachyo-ai
provider_slug: tachyo-ai
scheme_count: 1
schemes:
- evidence: Your Telegram account is your identity, and a short-lived code is how you prove it.
  how_to_obtain: Open @barryauthbot in Telegram and send /code; the bot replies with an 8‑character code.
  location: body
  name: Telegram short‑lived code
  type: other
slug: tachyo-ai-authentication
source_filename: tachyo-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.tachyo.ai/getting-started/signing-in
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.tachyo.ai/getting-started/signing-in\nsources:\n- https://docs.tachyo.ai/getting-started/signing-in\n- https://docs.tachyo.ai/platform/token-page\n- https://docs.tachyo.ai/platform/tokens\n- https://docs.tachyo.ai/getting-started/first-session\ndescription: Authentication is performed by obtaining a short‑lived 8‑character code from the Telegram bot @barryauthbot and submitting it on\n  the login page.\nschemes:\n- type: other\n  name: Telegram short‑lived code\n  evidence: Your Telegram account is your identity, and a short-lived code is how you prove it.\n  location: body\n  how_to_obtain: Open @barryauthbot in Telegram and send /code; the bot replies with an 8‑character code.\ndocs: https://docs.tachyo.ai/getting-started/signing-in\n"
source_yaml_url: https://artifacts.apis.io/tachyo-ai/authentication/tachyo-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Crypto
- Analytics
- Wallet
- Memecoin
---
