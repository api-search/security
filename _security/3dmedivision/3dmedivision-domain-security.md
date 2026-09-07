---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 3dmedivision.com
  spf: true
hosts:
- cert_expires: Nov 23 18:46:44 2026 GMT
  host: www.3dmedivision.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 3Dmedivision Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 3D Medivision, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 3D Medivision
provider_slug: 3dmedivision
slug: 3dmedivision-domain-security
source_filename: 3dmedivision-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.3dmedivision.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 18:46:44 2026 GMT\n  hsts: false\ndomains:\n- domain: 3dmedivision.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3dmedivision/refs/heads/main/security/3dmedivision-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Medical Devices
- Medical Imaging
- Surgical Video
- Veterinary
- Education
- Video On Demand
- Virtual Reality
- Health Care
- South Korea
---
