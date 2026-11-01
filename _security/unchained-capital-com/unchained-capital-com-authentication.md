---
anonymous_access: false
api_key_in: []
auth_types: []
description: Client authentication methods as described in Unchained help articles.
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Unchained Capital Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unchained Capital declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Unchained Capital
provider_slug: unchained-capital-com
scheme_count: 4
schemes:
- evidence: Use your email and password to sign in to your account at my.unchained.com .
  location: body
  name: Email and password
  type: other
- evidence: 'Passkeys (recommended): This security protocol requires a physical device, like a phone, computer, or Yubikey, to be present when you sign in.'
  header: Authorization
  how_to_obtain: Add a passkey via the Unchained account security tab following the on‑screen instructions.
  location: header
  name: Passkey (WebAuthn)
  type: other
- evidence: 'Authenticator apps (TOTP): An authenticator app such as Google Authenticator generates a time‑based code that you enter after your password.'
  how_to_obtain: Set up an authenticator app in the Security tab of your Unchained account and scan the QR code.
  location: body
  name: Authenticator app (TOTP)
  type: other
- evidence: The Unchained iOS app supports Face ID as a sign in method.
  how_to_obtain: Enable Face ID in the Unchained iOS app under Security and privacy → Manage Apple Face ID.
  location: device
  name: Face ID (biometric)
  type: other
slug: unchained-capital-com-authentication
source_filename: unchained-capital-com-authentication.yml
source_heading: Authentication Profile
source_url: https://help.unchained.com/how-do-i-reset-my-multi-factor-authentication-mfa
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.unchained.com/how-do-i-reset-my-multi-factor-authentication-mfa\nsources:\n- https://help.unchained.com/how-do-i-reset-my-multi-factor-authentication-mfa\n- https://help.unchained.com/how-do-i-set-up-multi-factor-authentication-mfa\n- https://help.unchained.com/how-do-i-enable-biometric-authentication-on-the-unchained-mobile-app\n- https://help.unchained.com/how-can-i-fix-hardware-wallet-signing-issues\ndescription: Client authentication methods as described in Unchained help articles.\nschemes:\n- type: other\n  name: Email and password\n  evidence: Use your email and password to sign in to your account at my.unchained.com .\n  location: body\n- type: other\n  name: Passkey (WebAuthn)\n  evidence: 'Passkeys (recommended): This security protocol requires a physical device, like a phone, computer, or Yubikey, to be present when\n    you sign in.'\n  location: header\n\
  \  header: Authorization\n  how_to_obtain: Add a passkey via the Unchained account security tab following the on‑screen instructions.\n- type: other\n  name: Authenticator app (TOTP)\n  evidence: 'Authenticator apps (TOTP): An authenticator app such as Google Authenticator generates a time‑based code that you enter after your\n    password.'\n  location: body\n  how_to_obtain: Set up an authenticator app in the Security tab of your Unchained account and scan the QR code.\n- type: other\n  name: Face ID (biometric)\n  evidence: The Unchained iOS app supports Face ID as a sign in method.\n  location: device\n  how_to_obtain: Enable Face ID in the Unchained iOS app under Security and privacy → Manage Apple Face ID.\ndocs: https://help.unchained.com/how-do-i-reset-my-multi-factor-authentication-mfa\n"
source_yaml_url: https://artifacts.apis.io/unchained-capital-com/authentication/unchained-capital-com-authentication.yml
summary_line: 4 schemes
tags:
- Bitcoin
- Financial Services
- Custody
- Investment
- Trust
---
