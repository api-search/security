---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 3dgsinc.com
  spf: true
hosts:
- cert_expires: Sep 21 04:27:12 2026 GMT
  host: www.3dgsinc.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 3D Glass Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 3D Glass Solutions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 3D Glass Solutions
provider_slug: 3d-glass-solutions
slug: 3d-glass-solutions-domain-security
source_filename: 3d-glass-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.3dgsinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 04:27:12 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: 3dgsinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3d-glass-solutions/refs/heads/main/security/3d-glass-solutions-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Semiconductors
- Advanced Packaging
- Glass Substrates
- RF Components
- Photonics
- Manufacturing
- Hardware
- Company
---
