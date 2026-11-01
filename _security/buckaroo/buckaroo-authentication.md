---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for the Buckaroo JSON API uses a standard HMAC scheme.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Buckaroo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Buckaroo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Buckaroo
provider_slug: buckaroo
scheme_count: 1
schemes:
- evidence: The authentication of this JSON API is based on a standard HMAC Authentication implementation.
  header: Authorization
  how_to_obtain: Website Key and Secret Key are obtained from the Buckaroo payment plaza (My Buckaroo → websites → {yourwebsite} for the Website Key and Configuration → Merchant → SecretKey for the Secret Key).
  location: header
  name: hmac
  type: hmac
slug: buckaroo-authentication
source_filename: buckaroo-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.buckaroo.io/docs/two-factor-authentication-2fa.md
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.buckaroo.io/docs/two-factor-authentication-2fa.md\nsources:\n- https://docs.buckaroo.io/docs/two-factor-authentication-2fa.md\n- https://docs.buckaroo.io/docs/riverty-strong-customer-authentication.md\n- https://docs.buckaroo.io/docs/json-authenticator.md\n- https://docs.buckaroo.io/docs/authentication-debugger.md\ndescription: Authentication for the Buckaroo JSON API uses a standard HMAC scheme.\nschemes:\n- type: hmac\n  name: hmac\n  evidence: The authentication of this JSON API is based on a standard HMAC Authentication implementation.\n  location: header\n  header: Authorization\n  how_to_obtain: Website Key and Secret Key are obtained from the Buckaroo payment plaza (My Buckaroo → websites → {yourwebsite} for the Website\n    Key and Configuration → Merchant → SecretKey for the Secret Key).\ndocs: https://docs.buckaroo.io/docs/two-factor-authentication-2fa.md\n"
source_yaml_url: https://artifacts.apis.io/buckaroo/authentication/buckaroo-authentication.yml
summary_line: 1 scheme
tags:
- Payments
- Online Payments
- In‑store Payments
- Omnichannel
- Credit Management
- Subscription Management
- Business Lending
- Payment Terminals
---
