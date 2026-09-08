---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: addx.co
  spf: true
hosts:
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: addx.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: api-docs.addx.co
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Addx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ADDX, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ADDX
provider_slug: addx
slug: addx-domain-security
source_filename: addx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: addx.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: false\n- host: api-docs.addx.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: addx.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/addx/refs/heads/main/security/addx-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Digital Securities Exchange
- Private Markets
- Tokenization
- Alternative Investments
- Wealth Management
- Capital Markets
- Fintech
- Digital Assets
- Investment Platform
- Singapore
---
