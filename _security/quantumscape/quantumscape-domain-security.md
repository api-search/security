---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: quantumscape.com
  spf: true
hosts:
- cert_expires: Aug 24 18:44:38 2026 GMT
  host: www.quantumscape.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quantumscape Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quantumscape, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Quantumscape
provider_slug: quantumscape
slug: quantumscape-domain-security
source_filename: quantumscape-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quantumscape.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 18:44:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: quantumscape.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quantumscape/refs/heads/main/security/quantumscape-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Battery
- Solid-State Batteries
- Energy Storage
- Electric Vehicles
- Clean Energy
- Manufacturing
---
