---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rayon.design
  spf: true
hosts:
- cert_expires: Sep  8 12:18:52 2026 GMT
  host: rayon.design
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rayon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rayon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Rayon
provider_slug: rayon
slug: rayon-domain-security
source_filename: rayon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rayon.design\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 12:18:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: rayon.design\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rayon/refs/heads/main/security/rayon-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Enterprise
- Artificial Intelligence
- CAD
- Architecture
- Design
- BIM
- Interior Design
- Collaboration
---
