---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@coinbase.com"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coinbase.com
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: docs.cdp.coinbase.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 01:17:33 2026 GMT
  host: api.cdp.coinbase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 05:30:25 2026 GMT
  host: api.coinbase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coinbase Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coinbase Global, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Coinbase Global
provider_slug: coinbase-global
slug: coinbase-global-domain-security
source_filename: coinbase-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.cdp.coinbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cdp.coinbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 01:17:33 2026 GMT\n  hsts: null\n- host: api.coinbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 05:30:25 2026 GMT\n  hsts: null\ndomains:\n- domain: coinbase.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@coinbase.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinbase-global/refs/heads/main/security/coinbase-global-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Blockchain
- Payments
- Wallets
- Trading
- Onchain
- Web3
- Financial Services
- Developer Platform
- AI Agents
- Stablecoins
---
