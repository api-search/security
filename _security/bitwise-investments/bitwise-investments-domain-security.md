---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bitwiseinvestments.com
  spf: true
hosts:
- cert_expires: Aug 19 13:26:49 2026 GMT
  host: bitwiseinvestments.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 10:52:54 2026 GMT
  host: developers.bitwiseinvestments.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 08:59:23 2026 GMT
  host: api.bitwiseinvestments.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitwise Investments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitwise Investments, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Bitwise Investments
provider_slug: bitwise-investments
slug: bitwise-investments-domain-security
source_filename: bitwise-investments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitwiseinvestments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 13:26:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.bitwiseinvestments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 10:52:54 2026 GMT\n  hsts: null\n- host: api.bitwiseinvestments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 08:59:23 2026 GMT\n  hsts: null\ndomains:\n- domain: bitwiseinvestments.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitwise-investments/refs/heads/main/security/bitwise-investments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Asset Management
- ETF
- Index Funds
- Market Data
- Financial Services
- Investment Management
---
