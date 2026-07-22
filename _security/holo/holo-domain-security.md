---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: holoam.com
  spf: true
hosts:
- cert_expires: Sep 10 04:02:07 2026 GMT
  host: holoam.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Holo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Holo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Holo
provider_slug: holo
slug: holo-domain-security
source_filename: holo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: holoam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 04:02:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: holoam.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/holo/refs/heads/main/security/holo-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Additive Manufacturing
- 3D Printing
- Metal 3D Printing
- Advanced Manufacturing
- Hardware
- Prototyping
---
