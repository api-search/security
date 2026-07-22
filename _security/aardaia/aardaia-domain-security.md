---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aardaia.com
  spf: false
hosts:
- cert_expires: Oct  5 21:52:48 2026 GMT
  host: aardaia.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aardaia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aardaia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: aardaia
provider_slug: aardaia
slug: aardaia-domain-security
source_filename: aardaia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aardaia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:52:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: aardaia.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aardaia/refs/heads/main/security/aardaia-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Agriculture
- AgTech
- Biotechnology
- Plant Breeding
- Genomics
- Food
- Netherlands
---
