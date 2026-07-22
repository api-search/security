---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cometaedu.com
  spf: false
hosts:
- cert_expires: Oct  8 16:17:17 2026 GMT
  host: cometaedu.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cometa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cometa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Cometa
provider_slug: cometa
slug: cometa-domain-security
source_filename: cometa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cometaedu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 16:17:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cometaedu.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cometa/refs/heads/main/security/cometa-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Education
- EdTech
- School Management
- SaaS
- Admissions
- Tuition Collections
- Communications
- Payments
- Mexico
---
