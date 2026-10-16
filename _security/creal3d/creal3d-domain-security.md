---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: creal.com
  spf: true
hosts:
- cert_expires: Nov 30 12:58:59 2026 GMT
  host: creal.com
  hsts: true
  hsts_max_age: 16000000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Creal3D Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Creal3d, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Creal3d
provider_slug: creal3d
slug: creal3d-domain-security
source_filename: creal3d-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: creal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 12:58:59 2026 GMT\n  hsts: true\n  hsts_max_age: 16000000\ndomains:\n- domain: creal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creal3d/refs/heads/main/security/creal3d-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Augmented Reality
- Light Field Display
- Display Technology
- Vision Care
---
