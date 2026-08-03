---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reflexion.com
  spf: true
hosts:
- cert_expires: Sep  5 03:23:45 2026 GMT
  host: reflexion.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reflexion Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RefleXion Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RefleXion Medical
provider_slug: reflexion-medical
slug: reflexion-medical-domain-security
source_filename: reflexion-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reflexion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 03:23:45 2026 GMT\n  hsts: false\ndomains:\n- domain: reflexion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reflexion-medical/refs/heads/main/security/reflexion-medical-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Medical Devices
- Oncology
- Radiation Oncology
- Radiotherapy
- Medical Imaging
- Cancer Care
---
