---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: calyxoinc.com
  spf: true
hosts:
- cert_expires: Nov 15 21:59:08 2026 GMT
  host: calyxoinc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Calyxo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Calyxo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Calyxo
provider_slug: calyxo
slug: calyxo-domain-security
source_filename: calyxo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: calyxoinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 21:59:08 2026 GMT\n  hsts: false\ndomains:\n- domain: calyxoinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calyxo/refs/heads/main/security/calyxo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Medical Devices
- Kidney Stone Care
- Healthcare
- Innovation
- Series F
---
