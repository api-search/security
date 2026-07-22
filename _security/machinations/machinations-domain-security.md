---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: machinations.io
  spf: true
hosts:
- cert_expires: Sep 24 01:05:17 2026 GMT
  host: machinations.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Machinations Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Machinations, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Machinations
provider_slug: machinations
slug: machinations-domain-security
source_filename: machinations-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: machinations.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 24 01:05:17 2026 GMT\n  hsts: false\ndomains:\n- domain: machinations.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/machinations/refs/heads/main/security/machinations-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Game Design
- Game Economy
- Simulation
- Tokenomics
- Game Development
- Modeling
- Gaming
---
