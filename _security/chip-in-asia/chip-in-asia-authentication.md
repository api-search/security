---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for CHIP Collect API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Chip In Asia Authentication
name_suffix: Authentication
oauth_flows: []
overview: CHIP declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CHIP
provider_slug: chip-in-asia
scheme_count: 2
schemes:
- evidence: 'Every request to the CHIP Collect API must include your Secret Key as a bearer token in the Authorization header: Authorization: Bearer <secret_key>'
  header: Authorization
  how_to_obtain: You can generate and manage your Secret Keys in the CHIP merchant portal.
  location: header
  name: Bearer
  type: http-bearer
- evidence: Verifying inbound webhook and success callback deliveries RSA signature in the X-Signature header
  header: X-Signature
  how_to_obtain: See Webhook signatures for the full algorithm, code samples, and how to obtain the public key.
  location: header
  name: RSA signature
  type: other
slug: chip-in-asia-authentication
source_filename: chip-in-asia-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.chip-in.asia/chip-collect/overview/authentication
source_yaml: "generated: '2026-10-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.chip-in.asia/chip-collect/overview/authentication\nsources:\n- https://docs.chip-in.asia/chip-collect/overview/authentication\ndescription: Authentication schemes for CHIP Collect API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Every request to the CHIP Collect API must include your Secret Key as a bearer token in the Authorization header: Authorization:\n    Bearer <secret_key>'\n  location: header\n  header: Authorization\n  how_to_obtain: You can generate and manage your Secret Keys in the CHIP merchant portal.\n- type: other\n  name: RSA signature\n  evidence: Verifying inbound webhook and success callback deliveries RSA signature in the X-Signature header\n  location: header\n  header: X-Signature\n  how_to_obtain: See Webhook signatures for the full algorithm, code samples, and how to obtain the public key.\ndocs: https://docs.chip-in.asia/chip-collect/overview/authentication\n"
source_yaml_url: https://artifacts.apis.io/chip-in-asia/authentication/chip-in-asia-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Finance
- Payments
- SME
- Malaysia
---
