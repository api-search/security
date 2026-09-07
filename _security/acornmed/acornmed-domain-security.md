---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: acornmed.com
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: en.acornmed.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Acornmed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acornmed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Acornmed
provider_slug: acornmed
slug: acornmed-domain-security
source_filename: acornmed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.acornmed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: acornmed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acornmed/refs/heads/main/security/acornmed-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Health
- Healthcare
- Life Sciences
- Biotechnology
- Genomics
- Diagnostics
- Oncology
- Precision Medicine
- Clinical Laboratory
- China
---
