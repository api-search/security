---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bgcg.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: fmxfutures.com
  spf: false
hosts:
- cert_expires: Sep 11 14:56:50 2026 GMT
  host: www.bgcg.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 14:47:12 2026 GMT
  host: www.fmxfutures.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 18:23:43 2026 GMT
  host: www.fenicsust.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bgc Partners Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BGC Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BGC Group
provider_slug: bgc-partners
slug: bgc-partners-domain-security
source_filename: bgc-partners-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bgcg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 14:56:50 2026 GMT\n  hsts: null\n- host: www.fmxfutures.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 14:47:12 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: www.fenicsust.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 18:23:43 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: bgcg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: fmxfutures.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bgc-partners/refs/heads/main/security/bgc-partners-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Brokerage
- Inter-Dealer Broker
- Financial Services
- Capital Markets
- Market Data
- Foreign Exchange
- Fixed Income
- Interest Rate Derivatives
- Energy And Commodities
- Equity Derivatives
- Credit Derivatives
- Futures Exchange
- SOFR
- US Treasuries
- Post-Trade
- Trading Infrastructure
- Financial Technology
- Fortune 1000
---
