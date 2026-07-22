---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: acxel.com
  spf: true
hosts:
- cert_expires: Aug 24 23:59:59 2026 GMT
  host: acxel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acxel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for acxel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: acxel
provider_slug: acxel
slug: acxel-domain-security
source_filename: acxel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acxel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: acxel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acxel/refs/heads/main/security/acxel-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Life Sciences
- Biotechnology
- Microfluidics
- Digital Biology
- Lab-on-Chip
- Drug Development
---
