---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aura.aero
  spf: true
hosts:
- cert_expires: Oct  3 04:43:03 2026 GMT
  host: aura.aero
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Auraaero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Auraaero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Auraaero
provider_slug: auraaero
slug: auraaero-domain-security
source_filename: auraaero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aura.aero\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 04:43:03 2026 GMT\n  hsts: false\ndomains:\n- domain: aura.aero\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auraaero/refs/heads/main/security/auraaero-domain-security.yml
summary_line: TLSv1.2
tags:
- EVTOL
- Aircraft
- Hybrid EVTOL
- Ultra‑Long Range
- Batteries
- Powercell
- Aviation
---
