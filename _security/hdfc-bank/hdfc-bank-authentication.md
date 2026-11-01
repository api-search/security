---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Hdfc Bank Authentication
name_suffix: Authentication
oauth_flows: []
overview: HDFC Bank declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: HDFC Bank
provider_slug: hdfc-bank
scheme_count: 2
schemes:
- description: One Time Password generation and validation for customer authentication.
  type: otp
- description: Token based authentication using ID token generated after NetBanking login.
  type: token
slug: hdfc-bank-authentication
source_filename: hdfc-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource:\n  - https://developer.hdfc.bank.in/otp-based-authentication\n  - https://developer.hdfc.bank.in/token-based-authentication\nschemes:\n  - type: otp\n    description: One Time Password generation and validation for customer authentication.\n  - type: token\n    description: Token based authentication using ID token generated after NetBanking login.\n"
source_yaml_url: https://artifacts.apis.io/hdfc-bank/authentication/hdfc-bank-authentication.yml
summary_line: 2 schemes
tags:
- Banking
- Finance
- India
- Payments
- OpenBanking
---
