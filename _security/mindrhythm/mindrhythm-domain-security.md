---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mindrhythm.com
  spf: true
hosts:
- cert_expires: Oct  2 22:51:02 2026 GMT
  host: mindrhythm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mindrhythm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MindRhythm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MindRhythm
provider_slug: mindrhythm
slug: mindrhythm-domain-security
source_filename: mindrhythm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mindrhythm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 22:51:02 2026 GMT\n  hsts: false\ndomains:\n- domain: mindrhythm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mindrhythm/refs/heads/main/security/mindrhythm-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Medical Devices
- Neurodiagnostics
- Neurology
- Stroke Detection
- Medical Technology
- Health
---
