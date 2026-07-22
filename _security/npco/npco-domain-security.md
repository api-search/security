---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: npco.ai
  spf: true
hosts:
- cert_expires: Aug 30 11:57:17 2026 GMT
  host: www.npco.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Npco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NPco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NPco
provider_slug: npco
slug: npco-domain-security
source_filename: npco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.npco.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 11:57:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: npco.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/npco/refs/heads/main/security/npco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Industrial, Energy & Iot
- Artificial Intelligence
- Physics Simulation
- Aerospace
- Defense
- Energy
- Engineering
- Simulation
---
