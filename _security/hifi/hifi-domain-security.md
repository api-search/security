---
api_specs:
- filename: hifi-account-api-openapi.yml
  format: yaml
  label: Hifi Account API
  slug: hifi-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-account-api-openapi.yml
- filename: hifi-common-api-openapi.yml
  format: yaml
  label: Hifi Common API
  slug: hifi-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-common-api-openapi.yml
- filename: hifi-cross-chain-bridge-api-openapi.yml
  format: yaml
  label: Hifi Cross-Chain Bridge API
  slug: hifi-cross-chain-bridge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-cross-chain-bridge-api-openapi.yml
- filename: hifi-crypto-transfer-api-openapi.yml
  format: yaml
  label: Hifi Crypto Transfer API
  slug: hifi-crypto-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-crypto-transfer-api-openapi.yml
- filename: hifi-file-api-openapi.yml
  format: yaml
  label: Hifi File API
  slug: hifi-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-file-api-openapi.yml
- filename: hifi-kyc-api-openapi.yml
  format: yaml
  label: Hifi Kyc API
  slug: hifi-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-kyc-api-openapi.yml
- filename: hifi-offramp-api-openapi.yml
  format: yaml
  label: Hifi Offramp API
  slug: hifi-offramp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-offramp-api-openapi.yml
- filename: hifi-onramp-api-openapi.yml
  format: yaml
  label: Hifi Onramp API
  slug: hifi-onramp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-onramp-api-openapi.yml
- filename: hifi-reporting-api-openapi.yml
  format: yaml
  label: Hifi Reporting API
  slug: hifi-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-reporting-api-openapi.yml
- filename: hifi-settlement-rules-api-openapi.yml
  format: yaml
  label: Hifi Settlement Rules API
  slug: hifi-settlement-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-settlement-rules-api-openapi.yml
- filename: hifi-token-swap-api-openapi.yml
  format: yaml
  label: Hifi Token Swap API
  slug: hifi-token-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-token-swap-api-openapi.yml
- filename: hifi-transfer-approvals-api-openapi.yml
  format: yaml
  label: Hifi Transfer Approvals API
  slug: hifi-transfer-approvals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-transfer-approvals-api-openapi.yml
- filename: hifi-user-api-openapi.yml
  format: yaml
  label: Hifi User API
  slug: hifi-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-user-api-openapi.yml
- filename: hifi-virtual-account-api-openapi.yml
  format: yaml
  label: Hifi Virtual Account API
  slug: hifi-virtual-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-virtual-account-api-openapi.yml
- filename: hifi-wallet-api-openapi.yml
  format: yaml
  label: Hifi Wallet API
  slug: hifi-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-wallet-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hifi.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hifibridge.com
  spf: true
hosts:
- cert_expires: Sep 30 13:59:03 2026 GMT
  host: hifi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 02:20:51 2026 GMT
  host: docs.hifi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 12:13:07 2026 GMT
  host: production.hifibridge.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hifi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hifi, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hifi
provider_slug: hifi
slug: hifi-domain-security
source_filename: hifi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hifi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 13:59:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.hifi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 02:20:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: production.hifibridge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 12:13:07 2026 GMT\n  hsts: null\ndomains:\n- domain: hifi.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: hifibridge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/security/hifi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Stablecoins
- Payments
- Money Movement
- On-Ramp
- Off-Ramp
- Crypto
- Fintech
- KYC
- Virtual Accounts
- Cross-Chain
- Financial Infrastructure
---
