---
api_specs:
- filename: ledger-swap-provider-openapi.yml
  format: yaml
  label: Ledger Wallet Exchange Provider APIs
  slug: ledger-wallet-exchange-provider-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledger/refs/heads/main/openapi/ledger-swap-provider-openapi.yml
- filename: ledger-enterprise-vault-openapi.yml
  format: yaml
  label: Ledger Enterprise API (Vault API)
  slug: ledger-enterprise-api-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledger/refs/heads/main/openapi/ledger-enterprise-vault-openapi.yml
- filename: ledger-enterprise-multisig-openapi.yml
  format: yaml
  label: Ledger Enterprise Multisig API
  slug: ledger-enterprise-multisig-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledger/refs/heads/main/openapi/ledger-enterprise-multisig-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ledger.com
  spf: true
hosts:
- cert_expires: Nov  5 13:52:53 2026 GMT
  host: www.ledger.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 21:17:31 2026 GMT
  host: developers.ledger.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:44:49 2026 GMT
  host: help.enterprise.ledger.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ledger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ledger, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ledger
provider_slug: ledger
slug: ledger-domain-security
source_filename: ledger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ledger.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 13:52:53 2026 GMT\n  hsts: false\n- host: developers.ledger.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 21:17:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.enterprise.ledger.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:44:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ledger.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ledger/refs/heads/main/security/ledger-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Digital Assets
- Hardware Wallet
- Self Custody
- Institutional Custody
- Blockchain
- Payments
- Staking
- Security
- Agent Skills
- agent-native
---
