---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 908devices.com
  spf: true
hosts:
- cert_expires: Oct 16 15:18:51 2026 GMT
  host: 908devices.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 908 Devices Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 908 Devices, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: 908 Devices
provider_slug: 908-devices
slug: 908-devices-domain-security
source_filename: 908-devices-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 908devices.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 15:18:51 2026 GMT\n  hsts: false\ndomains:\n- domain: 908devices.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/908-devices/refs/heads/main/security/908-devices-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Chemical Analysis
- Mass Spectrometry
- Spectroscopy
- Scientific Instruments
- Public Safety
- Defense
- Narcotics Detection
- Hazmat
- Hardware
- Life Sciences
---
