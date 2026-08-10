---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rejoni.com
  spf: true
hosts:
- cert_expires: Nov  3 01:12:35 2026 GMT
  host: rejoni.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rejoni Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rejoni, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rejoni
provider_slug: rejoni
slug: rejoni-domain-security
source_filename: rejoni-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rejoni.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 01:12:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rejoni.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rejoni/refs/heads/main/security/rejoni-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Medical Devices
- Women's Health
- Healthcare
- Biomaterials
- Life Sciences
- Surgery
- Clinical Trials
- MedTech
---
