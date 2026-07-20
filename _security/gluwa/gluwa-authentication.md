---
api_key_in:
- header
auth_types:
- apiKey
- http-signature
description: ''
kind: authentication
layout: security
method: searched
name: Gluwa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gluwa secures its APIs with apiKey and http-signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gluwa
provider_slug: gluwa
scheme_count: 2
schemes:
- credential_source: https://docs.gluwa.com/get-started/dashboard/api-keys.md
  description: API Key + Secret credential pair obtained from the Gluwa Dashboard (dashboard.gluwa.com/ApiKey). Used to authorize account-scoped requests such as creating payment requests. Sandbox and production keys are distinct.
  in: header
  name: Authorization
  parameter: Authorization
  type: apiKey
- description: Proof-of-ownership header used mainly on GET requests. Value is Base64Encode("<unix timestamp>.<Address Signature>"), where the address signature is produced with the wallet's private key.
  in: header
  name: X-REQUEST-SIGNATURE
  parameter: X-REQUEST-SIGNATURE
  signing_docs: https://docs.gluwa.com/development/creating-transaction-signatures.md
  type: apiKey
slug: gluwa-authentication
source_filename: gluwa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.gluwa.com/api/authentication.md\ndocs: https://docs.gluwa.com/api/authentication.md\nnotes: >-\n  No OpenAPI is published for the Gluwa REST API; this profile is captured from the\n  provider's documentation. Gluwa uses two request-authorization mechanisms depending\n  on the endpoint.\nsummary:\n  types: [apiKey, http-signature]\n  api_key_in: [header]\nschemes:\n  - name: Authorization\n    type: apiKey\n    in: header\n    parameter: Authorization\n    description: >-\n      API Key + Secret credential pair obtained from the Gluwa Dashboard\n      (dashboard.gluwa.com/ApiKey). Used to authorize account-scoped requests\n      such as creating payment requests. Sandbox and production keys are distinct.\n    credential_source: https://docs.gluwa.com/get-started/dashboard/api-keys.md\n  - name: X-REQUEST-SIGNATURE\n    type: apiKey\n    in: header\n    parameter: X-REQUEST-SIGNATURE\n    description: >-\n      Proof-of-ownership\
  \ header used mainly on GET requests. Value is\n      Base64Encode(\"<unix timestamp>.<Address Signature>\"), where the address\n      signature is produced with the wallet's private key.\n    signing_docs: https://docs.gluwa.com/development/creating-transaction-signatures.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gluwa/refs/heads/main/authentication/gluwa-authentication.yml
summary_line: apiKey/http-signature · 2 schemes
tags:
- Company
- Blockchain
- Cryptocurrency
- Stablecoin
- Payments
- Fintech
- Wallet
- Creditcoin
- Smart Contracts
- Emerging Markets
---
