---
api_key_in:
- header
api_specs:
- filename: paymate-global-partner-api-openapi.yml
  format: yaml
  label: PayMate Global Partner API
  slug: paymate-global-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymate/refs/heads/main/openapi/paymate-global-partner-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Paymate Authentication
name_suffix: Authentication
oauth_flows: []
overview: PayMate secures its APIs with apiKey across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PayMate
provider_slug: paymate
scheme_count: 0
schemes: []
slug: paymate-authentication
source_filename: paymate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://api.paymate.my/GlobalPartnerAPI (Authentication + Data Security sections); https://paymate.in/paymateapi/APIDoc.html (Authentication section)\ndocs:\n- https://api.paymate.my/GlobalPartnerAPI\n- https://paymate.in/paymateapi/APIDoc.html\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  self_service: false\n  note: >-\n    Neither PayMate API is self-service. Credentials for both are issued by PayMate after commercial\n    onboarding and KYC, and the India API additionally requires the calling domain or IP to be whitelisted.\napis:\n- api: PayMate Global Partner API\n  scheme: PartnerApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  verified: false\n  how_to_obtain: >-\n    \"The PayMate API uses secret API Key to authenticate requests. Partner/Merchant will get their secret\n    API Keys after successful onboarding by writing\
  \ to us at <regional support address>\" — Authentication\n    section of the Partner API documentation app. Regional addresses: support@paymate.sg, support@paymate.my,\n    support@paymate.ae, support@paymate.om, support@dunomo.au, support@dunomo.za.\n  evidence: >-\n    The exact header NAME is not published. An unauthenticated POST to https://api.paymate.my/v1/Countrylist\n    on 2026-08-26 returned HTTP 401 with {\"RequestID\":null,\"StatusCode\":\"106\",\"Description\":\"Empty/Invalid\n    header credentials\",\"DetailedSummary\":{}} — confirming header-carried credentials but not naming the\n    header. The `Authorization` header recorded in the OpenAPI securityScheme is our placeholder and is\n    marked x-verified false; confirm with PayMate before integrating.\n  transport_security: >-\n    \"The PayMate system will use hybrid encryption and decryption methodology. Hybrid encryption is the\n    combination of symmetric and asymmetric encryption\" — Data Security section. The key\
  \ exchange and\n    algorithm parameters are not published.\n- api: PayMate India Business Payments API (PMXClients)\n  scheme: MultiHeaderCredentials\n  type: apiKey\n  in: header\n  verified: true\n  parameters:\n  - name: MerchantIdentification\n    description: 32-digit alphanumeric merchant identifier issued by PayMate.\n    required: true\n  - name: TerminalIdentification\n    description: 32-digit alphanumeric terminal identifier issued by PayMate.\n    required: true\n  - name: XpressID\n    description: 10-digit alphanumeric PayMate account identifier.\n    required: true\n  - name: Email\n    description: >-\n      The registered signup email. Where an account has multiple users, passing that user's email applies\n      that user's role permissions; when absent the API assumes the Admin role.\n    required: true\n  payload_encryption: >-\n    Request and response JSON bodies are encrypted with AES-256 using a per-account key and IV published\n    in the account's Account Settings\
  \ > API Settings screen. The documentation states the key and IV can be\n    rotated by PayMate at any time.\n  network_controls: >-\n    The calling domain name or IP address must be whitelisted on the account before any call succeeds; error\n    code 192 is \"No Method Access for ip\" and 129 is \"Request from invalid Source\". The number of domains\n    permitted is a plan attribute (1 / 3 / 5 domains — see plans/paymate-plans-pricing.yml).\n  how_to_obtain: >-\n    Sign up, complete KYC verification, upgrade to a plan that includes API access, then whitelist the\n    calling domain/IP. Keys then appear under Account Settings > API Settings.\ngaps:\n- No OAuth 2.0, OpenID Connect or mTLS on either surface.\n- No published scope or permission model; authorization is role-based inside the PayMate account.\n- No published key-rotation procedure, key-prefix convention, or token expiry for the Global Partner API key.\n- The Global Partner API's credential header name is undocumented, so\
  \ an integrator cannot write a client\n  from the public documentation alone.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paymate/refs/heads/main/authentication/paymate-authentication.yml
summary_line: apiKey · 0 schemes
tags:
- Payments
- B2B Payments
- Accounts Payable
- Accounts Receivable
- Supply Chain Finance
- Invoice Discounting
- Working Capital
- Commercial Cards
- Financial Services
- India
- Fintech
- Company
---
