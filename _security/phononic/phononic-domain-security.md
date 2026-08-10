---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: phononic.com
  spf: true
hosts:
- cert_expires: Sep 14 15:57:20 2026 GMT
  host: phononic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Phononic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phononic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Phononic
provider_slug: phononic
slug: phononic-domain-security
source_filename: phononic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: phononic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:57:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: phononic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phononic/refs/heads/main/security/phononic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Semiconductors
- Hardware
- Cooling
- Thermal Management
- Data Center
- Artificial Intelligence
- Optoelectronics
- Sustainability
- Manufacturing
---
