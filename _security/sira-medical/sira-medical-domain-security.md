---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: siramedical.com
  spf: false
hosts:
- cert_expires: Sep  6 04:41:49 2026 GMT
  host: siramedical.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sira Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sira Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Sira Medical
provider_slug: sira-medical
slug: sira-medical-domain-security
source_filename: sira-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: siramedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 04:41:49 2026 GMT\n  hsts: false\ndomains:\n- domain: siramedical.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sira-medical/refs/heads/main/security/sira-medical-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Healthcare
- Medical Imaging
- Augmented Reality
- Surgical Planning
- Radiology
- Medical Devices
- Visualization
---
