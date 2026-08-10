---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: histosonics.com
  spf: true
hosts:
- cert_expires: Oct 23 10:02:27 2026 GMT
  host: histosonics.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Histosonics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HistoSonics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HistoSonics
provider_slug: histosonics
slug: histosonics-domain-security
source_filename: histosonics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: histosonics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 10:02:27 2026 GMT\n  hsts: null\ndomains:\n- domain: histosonics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/histosonics/refs/heads/main/security/histosonics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Healthcare
- Health Technology
- Oncology
- Focused Ultrasound
- Surgical Robotics
- Medical Imaging
---
