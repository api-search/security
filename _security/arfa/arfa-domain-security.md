---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arfatechnologies.com
  spf: true
hosts:
- cert_expires: Dec 12 05:35:44 2026 GMT
  host: arfatechnologies.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arfa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arfa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Arfa
provider_slug: arfa
slug: arfa-domain-security
source_filename: arfa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arfatechnologies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 05:35:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arfatechnologies.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arfa/refs/heads/main/security/arfa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web Development
- Digital Services
- Graphic Design
- E‑commerce
- New York
---
