---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: voommedicaldevices.com
  spf: true
hosts:
- cert_expires: Oct 30 02:24:25 2026 GMT
  host: www.voommedicaldevices.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Voom Medical Devices Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voom Medical Devices, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Voom Medical Devices
provider_slug: voom-medical-devices
slug: voom-medical-devices-domain-security
source_filename: voom-medical-devices-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.voommedicaldevices.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 02:24:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: voommedicaldevices.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voom-medical-devices/refs/heads/main/security/voom-medical-devices-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Medical Devices
- Health Care
- Orthopedics
- Surgery
- Medical Technology
- Manufacturing
---
