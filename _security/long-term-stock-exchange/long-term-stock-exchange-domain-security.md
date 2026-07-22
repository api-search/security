---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ltse.com
  spf: true
hosts:
- cert_expires: Sep 30 20:58:41 2026 GMT
  host: ltse.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Long Term Stock Exchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Long-Term Stock Exchange, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Long-Term Stock Exchange
provider_slug: long-term-stock-exchange
slug: long-term-stock-exchange-domain-security
source_filename: long-term-stock-exchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ltse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 20:58:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ltse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/long-term-stock-exchange/refs/heads/main/security/long-term-stock-exchange-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Stock Exchange
- Capital Markets
- Financial Services
- Market Data
- Trading
- Securities
- FIX Protocol
---
