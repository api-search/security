---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bmftec3d.com
  spf: false
hosts:
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: www.bmftec3d.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bmfprecision Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bmfprecision, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Bmfprecision
provider_slug: bmfprecision
slug: bmfprecision-domain-security
source_filename: bmfprecision-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bmftec3d.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bmftec3d.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bmfprecision/refs/heads/main/security/bmfprecision-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- 3D Printing
- Additive Manufacturing
- Precision Electronics
- Medical Devices
- Microfluidics
- Materials
- Custom Manufacturing
---
