---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dux.io
  spf: true
hosts:
- cert_expires: Sep 11 11:21:20 2026 GMT
  host: dux.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dux Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dux, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dux
provider_slug: dux
slug: dux-domain-security
source_filename: dux-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dux.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 11:21:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dux.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dux/refs/heads/main/security/dux-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cybersecurity
- Vulnerability Management
- Exposure Management
- Artificial Intelligence
- Agents
---
