---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wisk.aero
  spf: true
hosts:
- cert_expires: Sep 26 01:19:02 2026 GMT
  host: wisk.aero
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wisk Aero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wisk Aero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wisk Aero
provider_slug: wisk-aero
slug: wisk-aero-domain-security
source_filename: wisk-aero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wisk.aero\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 01:19:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wisk.aero\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wisk-aero/refs/heads/main/security/wisk-aero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advanced Air Mobility
- Aerospace
- Air Taxi
- Autonomy
- Boeing
- eVTOL
- Electric Aviation
- FAA Certification
- Self-Flying
- Urban Air Mobility
---
