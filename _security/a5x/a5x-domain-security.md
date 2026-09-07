---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: a5x.com.br
  spf: true
hosts:
- cert_expires: Dec  2 08:36:24 2026 GMT
  host: a5x.com.br
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: portal-tecnico.a5x.com.br
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: A5X Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for A5X, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: A5X
provider_slug: a5x
slug: a5x-domain-security
source_filename: a5x-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: a5x.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 08:36:24 2026 GMT\n  hsts: false\n- host: portal-tecnico.a5x.com.br\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: a5x.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/a5x/refs/heads/main/security/a5x-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial Services
- Capital Markets
- Stock Exchange
- Derivatives
- Futures
- Trading
- Market Data
- Clearing
- FIX Protocol
- Brazil
---
