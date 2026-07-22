---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: terminal-industries.com
  spf: true
hosts:
- cert_expires: Oct  8 21:36:50 2026 GMT
  host: terminal-industries.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Terminal Logistics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Terminal Logistics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Terminal Logistics
provider_slug: terminal-logistics
slug: terminal-logistics-domain-security
source_filename: terminal-logistics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: terminal-industries.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 21:36:50 2026 GMT\n  hsts: false\ndomains:\n- domain: terminal-industries.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terminal-logistics/refs/heads/main/security/terminal-logistics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Logistics
- Supply Chain
- Yard Management
- Computer Vision
- Artificial Intelligence
- Yard Operating System
---
