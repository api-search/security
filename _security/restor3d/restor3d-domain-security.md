---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: restor3d.com
  spf: true
hosts:
- cert_expires: Nov  5 05:24:23 2026 GMT
  host: www.restor3d.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Restor3D Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for restor3d, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: restor3d
provider_slug: restor3d
slug: restor3d-domain-security
source_filename: restor3d-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.restor3d.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 05:24:23 2026 GMT\n  hsts: false\ndomains:\n- domain: restor3d.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restor3d/refs/heads/main/security/restor3d-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Medical Devices
- Health
- Orthopedics
- 3D Printing
- Additive Manufacturing
- Implants
- Surgery
- Artificial Intelligence
- Manufacturing
- Company
---
