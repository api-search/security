---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jadu.io
  spf: false
hosts:
- cert_expires: Sep 27 16:53:43 2026 GMT
  host: jadu.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jadu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jadu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Jadu
provider_slug: jadu
slug: jadu-domain-security
source_filename: jadu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jadu.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 16:53:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: jadu.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jadu/refs/heads/main/security/jadu-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Cryptocurrency
- Trading
- Artificial Intelligence
- Automation
- Hyperliquid
- Decentralized Finance
---
