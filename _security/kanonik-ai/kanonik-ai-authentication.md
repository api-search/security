---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Kanonik
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Kanonik Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kanonik declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Kanonik
provider_slug: kanonik-ai
scheme_count: 3
schemes:
- evidence: Every workspace authenticates through Kanonik's identity service (OpenID Connect with PKCE).
  header: Authorization
  how_to_obtain: Sign in with your work email and password on the workspace sign‑in page; the system performs an OpenID Connect authorization flow with PKCE and returns a short‑lived bearer token used in the Authorization header.
  location: header
  name: OpenID Connect with PKCE
  type: http-bearer
- evidence: Your AI client connects over MCP using OAuth and registers itself automatically the first time it connect.
  how_to_obtain: The AI client initiates an OAuth flow with Kanonik’s identity service when first connecting via MCP; the client is automatically registered and receives an access token.
  name: MCP OAuth registration
  type: oauth2
- evidence: 'Kanonik uses time-based one-time passwords (TOTP) with any standard authenticator app: 1Password, Google Authenticator, Microsoft Authenticator, Authy, and similar.'
  how_to_obtain: Enroll by scanning a QR code presented at sign‑in; subsequent logins require entering the current TOTP code from the authenticator app.
  name: Time‑based One‑Time Password (TOTP) MFA
  type: other
slug: kanonik-ai-authentication
source_filename: kanonik-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://kanonik.ai/docs/getting-started/signing-up-and-your-trial/
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://kanonik.ai/docs/getting-started/signing-up-and-your-trial/\nsources:\n- https://kanonik.ai/docs/getting-started/signing-up-and-your-trial/\n- https://kanonik.ai/docs/account-and-security/accounts-sign-in-and-security/\n- https://kanonik.ai/docs/getting-started/getting-started-with-kanonik/\n- https://kanonik.ai/docs/getting-started/connecting-your-ai/\ndescription: Authentication methods for Kanonik\nschemes:\n- type: http-bearer\n  name: OpenID Connect with PKCE\n  evidence: Every workspace authenticates through Kanonik's identity service (OpenID Connect with PKCE).\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in with your work email and password on the workspace sign‑in page; the system performs an OpenID Connect authorization\n    flow with PKCE and returns a short‑lived bearer token used in the Authorization header.\n- type: oauth2\n  name: MCP\
  \ OAuth registration\n  evidence: Your AI client connects over MCP using OAuth and registers itself automatically the first time it connect.\n  how_to_obtain: The AI client initiates an OAuth flow with Kanonik’s identity service when first connecting via MCP; the client is automatically\n    registered and receives an access token.\n- type: other\n  name: Time‑based One‑Time Password (TOTP) MFA\n  evidence: 'Kanonik uses time-based one-time passwords (TOTP) with any standard authenticator app: 1Password, Google Authenticator, Microsoft\n    Authenticator, Authy, and similar.'\n  how_to_obtain: Enroll by scanning a QR code presented at sign‑in; subsequent logins require entering the current TOTP code from the authenticator\n    app.\ndocs: https://kanonik.ai/docs/getting-started/signing-up-and-your-trial/\n"
source_yaml_url: https://artifacts.apis.io/kanonik-ai/authentication/kanonik-ai-authentication.yml
summary_line: 3 schemes
tags:
- Security
- Compliance
- Artificial Intelligence
- Software-as-a-Service
- SOC 2
---
