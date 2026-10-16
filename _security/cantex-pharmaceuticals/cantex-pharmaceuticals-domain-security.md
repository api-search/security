---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cantex.com
  spf: true
hosts:
- cert_expires: Nov 30 12:07:58 2026 GMT
  host: cantex.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cantex Pharmaceuticals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cantex Pharmaceuticals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cantex Pharmaceuticals
provider_slug: cantex-pharmaceuticals
slug: cantex-pharmaceuticals-domain-security
source_filename: cantex-pharmaceuticals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cantex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 12:07:58 2026 GMT\n  hsts: false\ndomains:\n- domain: cantex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cantex-pharmaceuticals/refs/heads/main/security/cantex-pharmaceuticals-domain-security.yml
summary_line: TLSv1.3
tags:
- Biopharma
- Healthcare
- Florida
- ClinicalTrials
- Innovation
---
