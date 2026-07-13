---
api_specs:
- filename: openapi.json
  format: json
  label: Euler V3 Data API
  slug: euler-v3-data-api
  spec_type: OpenAPI
  url: https://v3.euler.finance/v3/openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "dns@euler.xyz"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: euler.finance
  spf: true
hosts:
- cert_expires: Sep  7 19:35:58 2026 GMT
  host: docs.euler.finance
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 15:43:49 2026 GMT
  host: v3.euler.finance
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 01:14:20 2026 GMT
  host: app.euler.finance
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Euler Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Euler Finance, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Euler Finance
provider_slug: euler
slug: euler-domain-security
source_filename: euler-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.euler.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 19:35:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: v3.euler.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 15:43:49 2026 GMT\n  hsts: null\n- host: app.euler.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 01:14:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: euler.finance\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"dns@euler.xyz\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/security/euler-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DeFi
- Lending
- Borrowing
- Finance
- Ethereum
- Blockchain
- Vaults
- Liquidation
- Interest Rates
- Permissionless
---
