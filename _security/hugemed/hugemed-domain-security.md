---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hugemed.net
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: hugemed.net
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hugemed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HugeMed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: HugeMed
provider_slug: hugemed
slug: hugemed-domain-security
source_filename: hugemed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hugemed.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: hugemed.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hugemed/refs/heads/main/security/hugemed-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Medical Devices
- Healthcare
- Endoscopy
- Airway Management
- Video Laryngoscope
- Medical Imaging
- MedTech
---
