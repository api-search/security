---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: gambit.trading
  spf: true
hosts:
- cert_expires: Jan 15 17:21:29 2027 GMT
  host: gambit.trading
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gambit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gambit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Gambit
provider_slug: gambit-trading
slug: gambit-trading-domain-security
source_filename: gambit-trading-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gambit.trading\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 17:21:29 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gambit.trading\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/gambit-trading/security/gambit-trading-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Artificial Intelligence
- Trading
- Hyperliquid
- MCP
---
