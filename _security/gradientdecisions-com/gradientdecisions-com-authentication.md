---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication is performed via payment using the x402 protocol; each request must include a payment attached to the call.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Gradient Decisions Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gradient Decisions declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Gradient Decisions
provider_slug: gradientdecisions-com
scheme_count: 1
schemes:
- evidence: Every call to the `check_merchant` MCP tool is authenticated by payment itself, per the x402 protocol
  name: x402 payment
  type: other
slug: gradientdecisions-com-authentication
source_filename: gradientdecisions-com-authentication.yml
source_heading: Authentication Profile
source_url: https://gradientdecisions.com/auth.md
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://gradientdecisions.com/auth.md\nsources:\n- https://gradientdecisions.com/auth.md\ndescription: Authentication is performed via payment using the x402 protocol; each request must include a payment attached to the call.\nschemes:\n- type: other\n  name: x402 payment\n  evidence: Every call to the `check_merchant` MCP tool is authenticated by payment itself, per the x402 protocol\ndocs: https://gradientdecisions.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/gradientdecisions-com/authentication/gradientdecisions-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Payments
- Fraud Prevention
- Merchants
- MCP
---
