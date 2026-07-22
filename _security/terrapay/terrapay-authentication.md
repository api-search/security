---
api_key_in:
- header
auth_types:
- apiKey
- custom-signed-headers
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Terrapay Authentication
name_suffix: Authentication
oauth_flows: []
overview: TerraPay secures its APIs with apiKey, custom-signed-headers, and mutualTLS across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TerraPay
provider_slug: terrapay
scheme_count: 6
schemes:
- description: Partner username (case-insensitive), issued at onboarding.
  in: header
  name: X-USERNAME
  sources:
  - https://developers.terrapay.com/docs/
  type: apiKey
- description: SHA-256 encoded partner password (case-insensitive).
  in: header
  name: X-PASSWORD
  sources:
  - https://developers.terrapay.com/docs/
  type: apiKey
- description: Request timestamp in "YYYY-MM-DD HH:mm:ss" format, UTC.
  in: header
  name: X-DATE
  sources:
  - https://developers.terrapay.com/docs/
  type: apiKey
- description: ISO Alpha-2 country code of the country where the transaction originates.
  in: header
  name: X-ORIGINCOUNTRY
  sources:
  - https://developers.terrapay.com/docs/
  type: apiKey
- description: For card (PAN) operations, the PAN is field-level encrypted with RSA/ECB/OAEPWithSHA-256 before being sent in this header.
  in: header
  name: X-PAN
  sources:
  - https://developers.terrapay.com/docs/
  type: apiKey
- description: All APIs require HTTPS with CA-issued SSL certificates; connectivity is over a site-to-site VPN tunnel or IP-whitelisted channel.
  name: mutual-tls
  sources:
  - https://developers.terrapay.com/getStarted.html
  type: mutualTLS
slug: terrapay-authentication
source_filename: terrapay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.terrapay.com/docs/ (Introduction / Developer Guide / Get Started)\nsummary:\n  types: [apiKey, custom-signed-headers, mutualTLS]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    TerraPay does not use OAuth2. Partners authenticate with a set of signed\n    request headers over a mutually-authenticated TLS channel (CA-issued SSL\n    certificates) reached via a site-to-site VPN tunnel or IP whitelist. API\n    credentials (username + password) are issued per partner during onboarding\n    and are distinct for each environment (Sandbox, UAT, LIVE); keys can be\n    reset/rotated in the developer portal.\nschemes:\n  - name: X-USERNAME\n    type: apiKey\n    in: header\n    description: Partner username (case-insensitive), issued at onboarding.\n    sources: [https://developers.terrapay.com/docs/]\n  - name: X-PASSWORD\n    type: apiKey\n    in: header\n    description: SHA-256 encoded partner password\
  \ (case-insensitive).\n    sources: [https://developers.terrapay.com/docs/]\n  - name: X-DATE\n    type: apiKey\n    in: header\n    description: Request timestamp in \"YYYY-MM-DD HH:mm:ss\" format, UTC.\n    sources: [https://developers.terrapay.com/docs/]\n  - name: X-ORIGINCOUNTRY\n    type: apiKey\n    in: header\n    description: ISO Alpha-2 country code of the country where the transaction originates.\n    sources: [https://developers.terrapay.com/docs/]\n  - name: X-PAN\n    type: apiKey\n    in: header\n    description: >-\n      For card (PAN) operations, the PAN is field-level encrypted with\n      RSA/ECB/OAEPWithSHA-256 before being sent in this header.\n    sources: [https://developers.terrapay.com/docs/]\n  - name: mutual-tls\n    type: mutualTLS\n    description: >-\n      All APIs require HTTPS with CA-issued SSL certificates; connectivity is\n      over a site-to-site VPN tunnel or IP-whitelisted channel.\n    sources: [https://developers.terrapay.com/getStarted.html]\n\
  key_management:\n  per_environment_keys: true\n  rotation: recommended (reset/regenerate in the developer portal on a rolling basis)\n  environments: [Sandbox, UAT, LIVE]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terrapay/refs/heads/main/authentication/terrapay-authentication.yml
summary_line: apiKey/custom-signed-headers/mutualTLS · 6 schemes
tags:
- Company
- Financial Services
- Payments
- Cross-Border Payments
- Remittances
- Mobile Money
- Digital Wallets
- Money Transfer
- Fintech
- GSMA Mobile Money API
---
