---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hallotheo.de
  spf: true
hosts:
- cert_expires: Sep  1 23:59:59 2026 GMT
  host: www.hallotheo.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hallo Theo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for hallo theo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: hallo theo
provider_slug: hallo-theo
slug: hallo-theo-domain-security
source_filename: hallo-theo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hallotheo.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hallotheo.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hallo-theo/refs/heads/main/security/hallo-theo-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Property Management
- Real Estate
- PropTech
- HOA Management
- Germany
- Facilities Management
---
