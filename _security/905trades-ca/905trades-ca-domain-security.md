---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 905trades.ca
  spf: true
hosts:
- cert_expires: Jan 26 06:35:39 2027 GMT
  host: 905trades.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 905Trades Ca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 905 Trades, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 905 Trades
provider_slug: 905trades-ca
slug: 905trades-ca-domain-security
source_filename: 905trades-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 905trades.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 06:35:39 2027 GMT\n  hsts: false\ndomains:\n- domain: 905trades.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/905trades-ca/security/905trades-ca-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Home Services
- Trade
- Canada
- GTA
---
