---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: plantdmaterials.com
  spf: true
hosts:
- cert_expires: Oct  3 03:34:59 2026 GMT
  host: www.plantdmaterials.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plantd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plantd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Plantd
provider_slug: plantd
slug: plantd-domain-security
source_filename: plantd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plantdmaterials.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 03:34:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: plantdmaterials.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plantd/refs/heads/main/security/plantd-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Building Materials
- Manufacturing
- Construction
- Sustainability
- Carbon Removal
- Climate Tech
- Advanced Materials
- Agriculture
---
