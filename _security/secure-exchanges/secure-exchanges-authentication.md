---
anonymous_access: false
api_key_in: []
auth_types: []
description: Secure Exchanges requires authentication to access returned documents, offering either an SMS code or sign‑in with a Microsoft account.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Secure Exchanges Authentication
name_suffix: Authentication
oauth_flows: []
overview: Secure Exchanges declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Secure Exchanges
provider_slug: secure-exchanges
scheme_count: 2
schemes:
- evidence: SMS code or Microsoft account
  name: SMS code
  type: other
- evidence: SMS code or Microsoft account
  name: Microsoft account
  type: other
slug: secure-exchanges-authentication
source_filename: secure-exchanges-authentication.yml
source_heading: Authentication Profile
source_url: https://www.secure-exchanges.com/secure-returns
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.secure-exchanges.com/secure-returns\nsources:\n- https://www.secure-exchanges.com/secure-returns\n- https://www.secure-exchanges.com/dmarc-authentication-guide\ndescription: Secure Exchanges requires authentication to access returned documents, offering either an SMS code or sign‑in with a Microsoft account.\nschemes:\n- type: other\n  name: SMS code\n  evidence: SMS code or Microsoft account\n- type: other\n  name: Microsoft account\n  evidence: SMS code or Microsoft account\ndocs: https://www.secure-exchanges.com/secure-returns\n"
source_yaml_url: https://artifacts.apis.io/secure-exchanges/authentication/secure-exchanges-authentication.yml
summary_line: 2 schemes
tags:
- Secure Document Exchange
- Email Encryption
- Digital Signatures
- Compliance
- File Transfer
---
