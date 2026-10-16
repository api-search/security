---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: curevo.in
  spf: true
hosts:
- cert_expires: Dec 18 11:43:57 2026 GMT
  host: curevo.in
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Curevo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curevo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Curevo
provider_slug: curevo
slug: curevo-domain-security
source_filename: curevo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: curevo.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 11:43:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: curevo.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curevo/refs/heads/main/security/curevo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Marketplace
- Biotechnology
- Global
- Telehealth
---
